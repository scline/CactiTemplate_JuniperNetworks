SNMP for SRX Central Point
------------------------------
This template goal is to gather interesting information about Juniper SRX Central Point.
This monitors all incoming sessions (also known as flows) before handing them off to an SPC card. For more information on this process please see http://www.juniper.net/techpubs/en_US/junos10.4/topics/concept/session-flow-central-point-for-srx-series-understanding.html.


Installing
----------
1)  Please copy the file juniper_srx_central_point.xml to <cacti directory>/resources/snmp_queries
2)  Import provided template(s) into cacti http://www.cacti.net/downloads/docs/html/template_import.html

Graphs
------
CP Sessions
	Displays the total amount of active sessions on an SRX unit, please not "max sessions" will generally be 0 on branch devices as this value means no-limit. Datacenter SRX units have this capped unless a license is purchased.

CP Sessions Per Second
	Shows the rate of sessions being created in an SRX device. 