
# By default don't host things inside the network

Internally we have the following servers running:

## spiderpig.pebblecode.net

This hosts the Working From Home API and the email cron that runs at 10am every weekday and appears in our inbox.

To get access to this server you'll need your ssh public key appended to: ~/.ssh/authorized_keys details: http://askubuntu.com/questions/46424/adding-ssh-keys-to-authorized-keys. Mention on slack you want access with your public key and someone will get back to you. 

You'll also need to add this to ~/.ssh/config: 

    Host spiderpig.pebblecode.net
    user pebble
    Port 7234

It's also a proxy server for routing traffic. For example, it routes [az-jenkins.pebblecode.net](az-jenkins.pebblecode.net) 
through to Snowball.

It's a Linux (Ubuntu) machine and it runs nginx.

## snowball

This is our Mac Mini which runs Jenkins and we use for building iOS (and Android) apps.

You can use [VNC](https://www.realvnc.com/download/viewer/) to access it. The IP address is 192.168.3.29. 
Ask on Slack for the password and someone should be able to send it to you.

## krusty

This is a mass storage device and is used by the design team to store documents. It is open to anyone. If you want to store documents on the network please ask [help@pebbleit.com](help@pebbleit.com) for access.

## sanjay.pebblecode.net

A windows server that handles DNS

## manjay.pebblecode.net

A legacy windows server 

## snowball.pebblecode.net

A mac mini used for iOS continuous integration

