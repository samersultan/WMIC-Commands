How old is your Windows install?

`wmic os get installdate`

List all programs that have Microsoft in the name

`wmic product where "name like '%microsoft%'" get name`

Uninstall everything that has toolbar in the name

`wmic product where "name like '%toolbar%'" call uninstall`

OEM model number

`wmic csproduct get name`

Motherboard model

`wmic baseboard get product`

Serial number/service tag

`wmic bios get serialnumber`

BIOS version

`wmic bios get SMBIOSBIOSVersion`

Get Printer Name, Port, 

`wmic printer get Name, Portname, Default`

Updates and Restart System 

`wuauclt /resetauthorization /detectnow /updatenow && shutdown /r /f /t 00`
