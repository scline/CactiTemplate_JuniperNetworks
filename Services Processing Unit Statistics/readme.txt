SNMP for SRX Services Processing Unit
-----------------------------------------
This template goal is to gather interesting information about Juniper SRX Services Processing Units. 

This monitors all active sessions (also known as flows) on each SPC and the CPU/Memory statistics of each card. This template should work for all models of Juniper SRX devices, even though branch models don't have a physical card they have built-in SPC processes and will show the same information.

Installing
----------
1)  Please copy the file juniper_srx_services_processing_unit.xml to <cacti directory>/resources/snmp_queries
2)  Import provided template(s) into cacti http://www.cacti.net/downloads/docs/html/template_import.html

Graphs
------
SPU Flow Sessions
	Displays the total amount of active sessions on an SPU unit and its maximum capacity. On branch devices there will only be 1 while datacenter models can have multiple cards installed.

SPU CPU
	Shows CPU utilization percentage of each SPU card.

SPU Memory
	Shows Memory utilization percentage of each SPU card.