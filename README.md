# hackintosh
NUC10i7FNH hackintosh. Perfect Wi-Fi support

## Config 
NUC10i7FNH

## OpenCore
[OpenCore0.7.3](https://github.com/acidanthera/OpenCorePkg)

## OS Version
11.6

## BIOS Config
- Advanced
	- Storage
		- SATA Mode Selection -> AHCI
	- Video
		- IGD Minimum Memory -> 64MB
		- IGD Aperture Size -> 256MB
		- IGD Primary Video Port -> Auto
- Boot
	- Secure Boot
		- Secure Boot -> Disabled
	- Boot Priority
		- UEFI Boot -> Checked
		- Legacy Boot -> Unchecked
		- Fast Boot -> Unchecked
- Power
	- Secondary Power Settings
		- Deep S4/S5 -> On
		- Wake on Lan from S4/S5 -> Stay Off
		- Wake System from S5 -> Off
		- Wake From Thunderbolt Device -> Off

## Wi-Fi
Support WPA/WPA2-Enterprise

## Airdrop
Work buggly

## To-Use
You have to update `config.plist`'s fields:
- PlatformInfo -> Generic -> MLB
- PlatformInfo -> Generic -> SystemSerialNumber
- PlatformInfo -> Generic -> SystemUUID

