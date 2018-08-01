# CryptoCowboy

A live working sample can be found here: http://computercowboy.tech/

Check out our Discord community: https://discord.gg/v6B7NsN

This is a beta release; Use at your own risk.


To start CryptoCowboy desktop version from Windows executable, simply open the executable. Note: This version automatically issues the 'Start' and 'Connect' commands so it is not nessesary to issue them manually via the web portal.

Start CryptoCowboy from CLI or Terminal:

sudo node index.js			-	Starts bot
sudo node index.js &		-	Starts bot and keeps bot running after closing terminal
sudo node index.js Start &	-	Starts bot and autotomates the setup process (Automatically issues the 'Connect' and 'Start' commands)

Deamon.js is an optional supplimentary software that helps automatically reboot CC when an issue occurs. If a timeout error occurs, deamon.js will issue a hard reset on CC.
To start Deamon.js in a separate terminal:

sudo node deamon.js &

Website GUI Commands:

Connect     -   Connects to XRPL API
Disconnect	-	Disconnects from XRPL API (Issue stop command before disconnecting)
Start       -   Begins autotrading (CC must be connected to XRPL first)
Stop		-	Stops autotrading
DropRange   -    Drops the range percentage by 1% (Keep above 1.5%)
BumpRange   -   Increases the range percentage by 1%

Linux - i.e Ubuntu
sudo pkill node                        -    Kills all node processes. Both index.js and deamon.js
sudo pkill -f "sudo node deamon.js"    -    Kills only deamon.js
