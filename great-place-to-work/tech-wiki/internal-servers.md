Internally we have the following servers running:

- spiderpig.pebblecode.net
  - This hosts working from home api and the email cron that runs at 10am every weekday and appears in our inbox.
  - To get access to this server you'll need your ssh public key appended to: ~/.ssh/authorized_keys details: http://askubuntu.com/questions/46424/adding-ssh-keys-to-authorized-keys. Mention on slack you want access with your public key and someone will get back to you. 
You'll also need to add this to ~/.ssh/config: 
Host spiderpig.pebblecode.net
user pebble
Port 7234
- please add more as you discover them
