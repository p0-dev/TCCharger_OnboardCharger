[FIRMWARE VERSION INFORMATION]

version : v1_oem
+ date : from the factory
	- baudrate: 250kbps
	- contains: node id 60 (3316) / 61 (3317) / 62 (3315)
	- required kl30 to be supplied with 12V
	- can message transmits when have CC and CP (charging station plugs in)
	- status: working ok as describe --> go to firmware for normal application

version : v2_non_kl30
	- baudrate: 250kbps
	- contains: node id 61 -> cannot be used as node 61 does not deal with CC and CP
	- required no kl30 to be supplied with 12V
	- can message transmits when have CC and CP (charing station plugs in)
	- status: work not ok with the application

version : v3_kl30_always-enable-can-message
+ date: 01.08.2023
	- baudrate: 250kbps
	- contains: node id 60 (3316)
	- required kl30 to be supplied with 12V
	- can message transmit when kl30 be supplied with 12V
	- status: cannot be used to re-charge

version : v4_kl30_always-enable-can-message
+ date: 04.08.2023
	- baudrate: 250kbps
	- contains: node id 60 (3316)
	- required kl30 to be supplied with 12V
	- can message transmit when kl30 be supplied with 12V
	- status: try to fix the problem with previous version, have not tested

version : v5_fix-CP-drop
+ date: 22.08.2023
	- baudrate: 250kbps
	- contains: node id 60 (3316)
	- required kl30 to be supplied with 12V
	- can message transmit when kl30 be supplied with 12V
	- status: try to fix the problem with drop CP signal during initialization or charging process