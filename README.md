# F5-REST---Platform-Builder
MS Excel Spreadsheet with Macros to build BIG-IP initial configuration via F5 REST api

There are 4 Worksheets (Sheet 1 - Configuration, REST, CURL and TMSH).  As you enter configuration parameters on Sheet 1 they are propogated to the REST, CURL and TMSH worksheets.

Authentication is performed using the X-F5-Auth-Token header and is supported in BIG-IP version 12.0 

The macros in this spreadsheet utilize the XMLHTTPREQUEST VB API and are unavailable on MAC or Linux platforms.
You will need to enable Macros in order to have the configuration pushed directly from the spreadsheet.

The BIG-IP device (Physical or virtual) will need to be licensed and have an address assigned to the managment port.

Objects set or created:
- Hostname
- NTP
- TimeZone
- DNS resolver
Network Objects:
- VLANS
- Self IPs
- Default Route

It can optionally create base profiles:

  Profiles
  - TCP
  - UDP
  - HTTP
  - ClientSSL
  - ServerSSL
  - OneConnect

  Monitors:
  - HTTP_HEAD
  - HTTPS_HEAD
  - TCP


You have the options to Deploy configuration, Create UCS, Create SCF and Load default configuration.
