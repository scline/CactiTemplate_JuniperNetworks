CactiTemplate-Juniper_Firewall_Filter
=====================================

This SNMP Query allows us to graph and display the "show firewall" command from a JunOS device. This was tested on EX and SRX series devices though should work across all JunOS platforms. 
For more information on the command itself please check out http://www.juniper.net/techpubs/en_US//junos/topics/reference/command-summary/show-firewall-filter.html

Installation
1) copy "Juniper_Firewall_Filter.xml" to your <cacti_directory>/resource/snmp_queries/
2) Import the provided template "cacti_data_query_juniper_-_firewall_filter_stats.xml" to cacti. This was originally exported using Cacti 0.8.7i.