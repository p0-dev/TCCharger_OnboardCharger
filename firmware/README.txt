[FIRMWARE VERSION INFORMATION]

version : original
+ date : from the factory
	- baudrate: 250kbps
	- contains: node id 60 (3316) / 61 (3317) / 62 (3315)
	- required kl30 to be supplied with 12V
	- can message transmits when have CC and CP (charging station plugs in)
	- status: working ok as describe --> go to firmware for normal application

version : non_kl30
	- baudrate: 250kbps
	- contains: node id 61 -> cannot be used as node 61 does not deal with CC and CP
	- required no kl30 to be supplied with 12V
	- can message transmits when have CC and CP (charing station plugs in)
	- status: work not ok with the application

version : v1
+ date: 01.08.2023
	- baudrate: 250kbps
	- contains: node id 60 (3316)
	- required kl30 to be supplied with 12V
	- can message transmit when kl30 be supplied with 12V
	- status: N/A