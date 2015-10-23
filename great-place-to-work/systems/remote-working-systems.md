# Remote Working systems

##VPN

### Prerequisites

- Username/Password - If you haven't already been given this when you started raise a support ticket with pebble IT ( [http://support.pebbleit.com](http://www.google.com/url?q=http%3A%2F%2Fsupport.pebbleit.com%2F&sa=D&sntz=1&usg=AFrqEzc8tVVA8Iz1kcZbyPw_mjYiTxK9IQ) and google login)
- Shared secret - This is stored in Mortimer. Either make a note of it when your in the office or ask one of your colleagues very nicely to look it up for you as its only accessible in the local network.

### Default windows setup
 
Some people have issues setting up the default windows VPN. The other alternative is to use the sonicwall one (detailed later in this document).

Search for the VPN setup wizzard

![capture](https://cloud.githubusercontent.com/assets/753089/10696674/2a91e908-79a1-11e5-8578-9742457356ae.png)

Enter ex01.pebbleit.com as the internet address

![capture2](https://cloud.githubusercontent.com/assets/753089/10696676/2df2bb18-79a1-11e5-8259-e7bcf6743822.png)

Follow the rest of the wizzard, entering your username and password. It will try to connect but wont be able to

![capture3](https://cloud.githubusercontent.com/assets/753089/10696680/311a225e-79a1-11e5-8a3d-fc08c8d160f2.png)

Navigate to your new vpn in the network connections and click properties on it. Enter ex01.pebbleit.com as the hosthane and vpn type to L2TP. In advanced settings enter the pre shared key.

![capture5](https://cloud.githubusercontent.com/assets/753089/10696684/3550152c-79a1-11e5-8131-c5c364c6ca43.png)

![capture6](https://cloud.githubusercontent.com/assets/753089/10696687/390d81cc-79a1-11e5-8609-b3f7e39a6f27.png)

You should now be able to connect!

If you get a message something like "L2TP connection attempt failed because the security layer encountered a processing error during initial negotiations with the remote computer" then follow the instructions on[ this page](https://support.microsoft.com/en-us/kb/926179) and be sure to restart your computer.

[SonicWall VPN](https://www.google.com/url?q=https%3A%2F%2Fpebbleit.zendesk.com%2Fattachments%2Ftoken%2Fglbglkzvzjkw0n3%2F%3Fname%3D184-001457-00_Rev_A_GVCSetup64.exe&sa=D&sntz=1&usg=AFrqEzf1JdalT5v_1TmEp3YILgqljfv3EQ) setup

Install the [SonicWall VPN client](https://www.google.com/url?q=https%3A%2F%2Fpebbleit.zendesk.com%2Fattachments%2Ftoken%2Fglbglkzvzjkw0n3%2F%3Fname%3D184-001457-00_Rev_A_GVCSetup64.exe&sa=D&sntz=1&usg=AFrqEzf1JdalT5v_1TmEp3YILgqljfv3EQ) (link is for 64bit version). Use the VPN secret key (see Mortimer-&gt;pebble{code}, only accessible from pebble network until you have VPN configured!) and your username/password.  To request a VPN login, submit a support request at[http://support.pebbleit.com](http://www.google.com/url?q=http%3A%2F%2Fsupport.pebbleit.com&sa=D&sntz=1&usg=AFrqEzcQpdH7ke7sI6YMdcGzpK-OXH1MuA) using your pebblecode.com google login.

![vpn1](https://cloud.githubusercontent.com/assets/753089/10696688/3d39060e-79a1-11e5-94af-5434f2778eb3.png)
![vpn2](https://cloud.githubusercontent.com/assets/753089/10696689/3d49bad0-79a1-11e5-9703-b7de69a92873.png)
![vpn3](https://cloud.githubusercontent.com/assets/753089/10696690/3d5551ec-79a1-11e5-94be-17ae6c85bb62.png)

## Campfire

Try not to have conversations via chat if they may be useful for the entire team. Start them on Slack, and move to a hangout if appropriate.

The Flare desktop client is very flaky - notifications stop working at random times. I've had much more success with the web client + [kindling](https://chrome.google.com/webstore/detail/abnakpmgckdkcpgbcejajjbllagggcif) for notifications.

## Hangouts

Far more productive than typing extended conversations. Summarise on Slack if the whole team would benefit.

## Shared Calendar

Share your gmail calendar. This will inform other team members when there are some official holidays and annual leave.
