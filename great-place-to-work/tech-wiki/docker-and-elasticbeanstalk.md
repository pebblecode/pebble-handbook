# Docker and Elastic Beanstalk

Developing docker images that are deployable on ElasticBeanstalk has some steps,
but is relativly easy to implement.

## Set up Amazon

The first step is to set up the requirements in the Amazon console. First go to
`Services > IAM` and `Create New Group`. Once the group has been created, create
users if there are no existing users and download their credential files.

**IT IS VERY IMPORTANT YOU GRAB THESE NOW.**

Put each user into the group and make sure you share the AWS key and secret with
the user.  Finally give each group permissions.  The recommended permissions
are:

```
AmazonRDSFullAccess
AmazonS3FullAccess
AWSElasticBeanstalkFullAccess
CloudWatchLogsFullAccess
```

Next, go to `Servies > EC2` and in the sidebar select `Key Pairs` and create a
new keypair.  Once created it will download a .pem file.  MAKE SURE YOU KEEP
THIS FILE IN A SAFE PLACE AND DISTRIBUTE TO ALL TEAM MEMBERS.

## Set up access in your environment.

First you need to make sure you have the ElasicBeanstalk tools set up on your
machine, this is installed with python pip (you may have to run this as sudo)

```
pip install awsebcli [--upgrade]
```

Once installed, in you home folder go to `~/.aws` and create a `credentials`
file:

```
[<profilename>]
aws_access_key_id = <your AWS KEY>
aws_secret_access_key = <your AWS SECRET>
```

Next, create a `config` file:

```
[profile votesforschools]
region=eu-west-1
output=json
```

Now in your project root folder, you can create a `Dockerfile` and a
`Dockerrun.aws.json` file.

* [Dockerfile file documentation](https://docs.docker.com/reference/builder/)
* [Dockerrun.aws.json documentation](http://docs.aws.amazon.com/elasticbeanstalk/latest/dg/create_deploy_docker_image.html)

An example Dockerfile might look like:

```
FROM node:wheezy

EXPOSE 9000 80 443

ENV APP_DIR /opt/my-app

WORKDIR ${APP_DIR}

ADD . $APP_DIR

RUN apt-get update && apt-get install -y procps

RUN npm install

RUN npm run build

#CMD ["npm", "start"]
```

An example Dockerrun.aws.json might look like:

```
{
  "AWSEBDockerrunVersion": "1",
  "Authentication": {
    "Bucket": "bucket-name",
    "Key": "path/to/config"
  },
  "Image": {
    "Name": "project/appname:latest",
    "Update": "true"
  },
  "Ports": [{
    "ContainerPort": "9000"
  }, {
    "ContainerPort": "80"
  },{
    "ContainerPort": "443"
  }]
}
```

## Setting up ElasticBeanstalk Instances

Once you have your project running locally, you can now type `eb init 
--profile profilename`.  Follow the options for it, and confirm it is using
docker.

Next you want to create an instance and deploy.

`eb create`

For docker it's recommended you may want to use a larger instance than a 
`t1.micro`

`eb create --instance_type m3.medium`

You will be asked some questions around creating the environment name and CNAME
record for this instance.

This will deploy the current branch to your instance.  When you make further
changes, you can then just type `eb deploy`.  If you want to use a different
branch at this point, first type `eb use <environment name>` before deploy.