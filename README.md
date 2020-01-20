# PFSense-Suricata-ELK
Pipelines for ELK 7.x with PFSense 2.4.4 &amp; Suricata<br/>
Initial examples pulled from Patrick Jennings & 3ilson<br/>
https://github.com/patrickjennings/logstash-pfsense<br/>
http://pfelksuricata.3ilson.com/<br/>
<br/>
Currently version 2.4.4 of PFSense using Patrick Jennings filters fails with ICMPv6 messages, and neither his nor 3ilson's examples successfully parse PFSense integrated Suricata syslog messages.<br/>
To utilize in your setup, replace any lines with triple asterisks, with your correct IP and remove the asterisks.<br/>
There are probably far more graceful methods for parsing the log data, but after failing to find examples that work with current software versions this is what I found to work on my setup.<br/>
Be sure to update 11-pfsense.conf line 13 with your correct timezone.<br/>
<br/>
These examples are provided in the hope that it may save others time when building their own setups. <br/>
