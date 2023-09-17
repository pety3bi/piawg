Copy the script to your router. Run the following command, I'm assuming you called the file pia_wg.sh. This will make the script executable and also ensure it is kept after a sysupgrade.

chmod +x /root/piawgx.sh
echo "/root/piawgx.sh" >> /etc/sysupgrade.conf

Install dependencies

opkg update
opkg install jq 
opkg install curl

Run the script for the first time

/root/piawgx.sh
