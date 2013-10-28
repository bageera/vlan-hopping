Frogger - VLAN Hopping
============================================

Simple VLAN enumeration and hopping script.

Released as open source by NCC Group Plc - http://www.nccgroup.com/

Developed by Daniel Compton, daniel dot compton at nccgroup dot com

https://github.com/nccgroup/vlan-hopping

Released under AGPL see LICENSE for more information

ported over to python

Installing  
=======================
    git clone https://github.com/nccgroup/vlan-hopping.git


How To Use	
=======================
    ./frogger.py

Run as root.

Features	
=======================

* Sniffs out CDP packets and extracts (VTP domain name, VLAN management address, Native VLAN ID and IOS version of Cisco devices)
* It will enable a DTP trunk attack automatically
* Sniffs out and extracts all 802.1Q tagged VLAN packets within STP packets and extracts the unique IDs.
* Auto arp-scans the discovered VLAN IDs and auto tags packets and scans each VLAN ID for live devices.
* Auto option to auto create a VLAN interface within the found network to connect to that VLAN.

Requirements   
=======================
* scapy
* sqlite3
* socket
* fcntl
* struct
* array



