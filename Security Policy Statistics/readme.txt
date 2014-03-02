SNMP for SRX Security Policies
------------------------------
This template goal is to gather interesting information about Juniper SRX security policies. In order for this data to populate each policy monitored must have counters enabled. This is accomplished by enabling "then count". 
http://jsrx.juniperwiki.com/index.php?title=Policies#Then_Action

You can validate this from cacti by looking at the "Stats Availability" before making the graph. This should equal 1 for data to populate. If your device is not set to count this value will equal 2.

SNMP MIB Reference 
http://www.juniper.net/techpubs/en_US/junos10.1/information-products/topic-collections/config-guide-network-mgm/mib-jnx-js-policy.txt

Installing
----------
1)  Please copy the file juniper_srx_security_policy.xml to <cacti directory>/resources/snmp_queries
2)  Import provided template(s) into cacti http://www.cacti.net/downloads/docs/html/template_import.html

Graphs
------
Security Policy Lookups
    Shows the amount of policy lookups that occurred on the security policy.
    http://www.juniper.net/techpubs/en_US/junos12.1/topics/concept/security-user-role-policy-lookup-understanding.html

Security Policy Sessions
    Shows the number of current active sessions (also known as flows) that a Security Policy is currently using.

Security Policy Traffic
    Displays the amount of traffic currently being processed by a Security Policy. Please note if the policy is set to drop traffic you will only get Inbound data since the policy drops the outbound traffic (like it should :])

Security Policy Packets
    Same as Traffic graph but instead of Bits per Second this is showing Packet per Second on a Security Policy.