# Remote Working systems

##VPN

### Prerequisites

- Username/Password - If you haven't already been given this when you started raise a support ticket with pebble IT ( [http://support.pebbleit.com](http://www.google.com/url?q=http%3A%2F%2Fsupport.pebbleit.com%2F&sa=D&sntz=1&usg=AFrqEzc8tVVA8Iz1kcZbyPw_mjYiTxK9IQ) and google login)
- Shared secret - This is stored in Mortimer. Either make a note of it when your in the office or ask one of your colleagues very nicely to look it up for you as its only accessible in the local network.

### Default windows setup
 
Some people have issues setting up the default windows VPN. The other alternative is to use the sonicwall one (detailed later in this document).

Search for the VPN setup wizzard

Enter ex01.pebbleit.com as the internet address

Follow the rest of the wizzard, entering your username and password. It will try to connect but wont be able to

Navigate to your new vpn in the network connections and click properties on it. Enter ex01.pebbleit.com as the hosthane and vpn type to L2TP. In advanced settings enter the pre shared key.

You should now be able to connect!

If you get a message something like "L2TP connection attempt failed because the security layer encountered a processing error during initial negotiations with the remote computer" then follow the instructions on[ this page](https://support.microsoft.com/en-us/kb/926179) and be sure to restart your computer.

[SonicWall VPN](https://www.google.com/url?q=https%3A%2F%2Fpebbleit.zendesk.com%2Fattachments%2Ftoken%2Fglbglkzvzjkw0n3%2F%3Fname%3D184-001457-00_Rev_A_GVCSetup64.exe&sa=D&sntz=1&usg=AFrqEzf1JdalT5v_1TmEp3YILgqljfv3EQ) setup

Install the [SonicWall VPN client](https://www.google.com/url?q=https%3A%2F%2Fpebbleit.zendesk.com%2Fattachments%2Ftoken%2Fglbglkzvzjkw0n3%2F%3Fname%3D184-001457-00_Rev_A_GVCSetup64.exe&sa=D&sntz=1&usg=AFrqEzf1JdalT5v_1TmEp3YILgqljfv3EQ) (link is for 64bit version). Use the VPN secret key (see Mortimer-&gt;pebble{code}, only accessible from pebble network until you have VPN configured!) and your username/password.  To request a VPN login, submit a support request at[http://support.pebbleit.com](http://www.google.com/url?q=http%3A%2F%2Fsupport.pebbleit.com&sa=D&sntz=1&usg=AFrqEzcQpdH7ke7sI6YMdcGzpK-OXH1MuA) using your pebblecode.com google login.

## Campfire

Try not to have conversations via chat if they may be useful for the entire team. Start them on Slack, and move to a hangout if appropriate.

The Flare desktop client is very flaky - notifications stop working at random times. I've had much more success with the web client + [kindling](https://chrome.google.com/webstore/detail/abnakpmgckdkcpgbcejajjbllagggcif) for notifications.

## Hangouts

Far more productive than typing extended conversations. Summarise on Slack if the whole team would benefit.

## Shared Calendar

Share your gmail calendar. This will inform other team members when there are some official holidays and annual leave.
