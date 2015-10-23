
# By default don't host things inside the network

Internally we have the following servers running:

## spiderpig.pebblecode.net

This hosts working from home api and the email cron that runs at 10am every weekday and appears in our inbox.

To get access to this server you'll need your ssh public key appended to: ~/.ssh/authorized_keys details: http://askubuntu.com/questions/46424/adding-ssh-keys-to-authorized-keys. Mention on slack you want access with your public key and someone will get back to you. 

You'll also need to add this to ~/.ssh/config: 

    Host spiderpig.pebblecode.net
    user pebble
    Port 7234

## krusty

This is a mass storage device and is used by the design team to store documents. It is open to anyone. If you want to store documents on the network please ask [help@pebbleit.com](help@pebbleit.com) for access.

## sanjay.pebblecode.net

A windows server that handles DNS

## manjay.pebblecode.net

A legacy windows server 

## snowball.pebblecode.net

A mac mini used for iOS continuous integration

