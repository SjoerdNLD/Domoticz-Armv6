Armv6 build of Domoticz. Using stable release source from https://github.com/domoticz/domoticz/releases/
It can be used on th raspberry pi B+ v1.2 (which supports only Armv6)

You can transfer the file using WinSCP https://winscp.net/eng/download.php
Or download it directly:
```markdown
wget https://github.com/SjoerdNLD/Domoticz-Armv6/releases/download/xx-version-xx/domoticz_linux_xx-version-xx_armv6.tgz

Example: wget https://github.com/SjoerdNLD/Domoticz-Armv6/releases/download/2024.4/domoticz_linux_2024.4_armv6.tgz
```

To update a running install: 
Stop, unpack and start using the following commands:
```markdown
sudo service domoticz.sh stop 
sudo tar -xzvf domoticz_linux_xx-version-xx_armv6.tgz 
sudo service domoticz.sh start 
rm domoticz_linux_xx-version-xx_armv6.tgz
```

For a new install:
Unpack, register and start using the following commands:
```markdown
sudo tar -xzvf domoticz_linux_xx-version-xx_armv6.tgz
sudo cp domoticz.sh /etc/init.d
sudo chmod +x /etc/init.d/domoticz.sh
sudo update-rc.d domoticz.sh defaults
sudo service domoticz.sh start 
rm domoticz_linux_xx-version-xx_armv6.tgz
```
Please view the license here https://github.com/domoticz/domoticz/blob/development/License.txt
