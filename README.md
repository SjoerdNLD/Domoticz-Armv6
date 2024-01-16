Armv6 build of Domoticz. Using stable release source from https://github.com/domoticz/domoticz/releases/

You can transfer the file using WinSCP https://winscp.net/eng/download.php

Stop, unpack and start using the following commands:

```markdown
sudo service domoticz.sh stop 
tar -xzvf domoticz_linux_xx-version-xx_armv6.tgz 
sudo service domoticz.sh start 
rm domoticz_linux_xx-version-xx_armv6.tgz
```

Please view the license here https://github.com/domoticz/domoticz/blob/development/License.txt
