# PFSense-Suricata-ELK
Pipelines for ELK 7.x with PFSense 2.4.4 &amp; Suricata
Initial examples pulled from Patrick Jennings & 3ilson
https://github.com/patrickjennings/logstash-pfsense
http://pfelksuricata.3ilson.com/

Currently version 2.4.4 of PFSense using Patrick Jennings filters fails with ICMPv6 messages, and neither his nor 3ilson's examples successfully parse PFSense integrated Suricata syslog messages.
To utilize in your setup, replace any lines with ***sample IP*** with your correct IP and remove the asterisks.
There are probably far more graceful methods for parsing the log data, but after failing to find examples that work with current software versions this is what I found to work on my setup.
Be sure to update 11-pfsense.conf line 13 with your correct timezone.

These examples are provided in the hope that it may save others time when building their own setups. 
