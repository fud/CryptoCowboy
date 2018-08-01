# CryptoCowboy

A live working sample can be found here: http://computercowboy.tech/

Check out our Discord community: https://discord.gg/v6B7NsN

This is a beta release; Use at your own risk.

<br><br>

To start CryptoCowboy desktop version from Windows executable, simply open the executable. Note: This version automatically issues the 'Start' and 'Connect' commands so it is not nessesary to issue them manually via the web portal.
<br><br>
<b>Start CryptoCowboy from Linux Terminal:</b>
<br><br>
sudo node index.js			-	Starts bot
<br>
sudo node index.js &		-	Starts bot and keeps bot running after closing terminal
<br>
sudo node index.js Start &	-	Starts bot and autotomates the setup process (Automatically issues the 'Connect' and 'Start' commands)
<br>
<br>
Deamon.js is an optional supplimentary software that helps automatically reboot CC when an issue occurs. If a timeout error occurs, deamon.js will issue a hard reset on CC.
<br>
<br>
<b>To start Deamon.js in a separate terminal:</b>
<br>
<br>
sudo node deamon.js &
<br>
<br>
<b>Website GUI Commands:</b>
<br>
<br>

Connect     -   Connects to XRPL API
<br>
Disconnect	-	Disconnects from XRPL API (Issue stop command before disconnecting)
<br>
Start       -   Begins autotrading (CC must be connected to XRPL first)
<br>
Stop		-	Stops autotrading
<br>
DropRange   -    Drops the range percentage by 1% (Keep above 1.5%)
<br>
BumpRange   -   Increases the range percentage by 1%
<br>
<br>
<b>Linux - i.e Ubuntu</b>
<br>
sudo pkill node                        -    Kills all node processes. Both index.js and deamon.js
<br>
sudo pkill -f "sudo node deamon.js"    -    Kills only deamon.js
<br>
