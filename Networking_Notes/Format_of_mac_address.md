# Format of MAC address 
* It is 12 digits or 6-byte hexadecimal number, which is represented in colon-hexadecimal notation format. It is divided into six octets, and each octet contains 8 bits. 
* The first three octets are used as the OUI or Organizationally Unique Identifier. These MAC prefixes are assigned to each organization or vendor by the IEEE Registration Authority Committee. 

---
* Some example of OUI of known vendors are: 
  * CC:46:D6 - Cisco 
  * 3C:5A:B4 - Google, Inc. 
  * 3C:D9:2B - Hewlett Packard 
  * 00:9A:CD - HUAWEI TECHNOLOGIES CO.,LTD 
--- 
 
* The last three octets are NIC specific and used by the manufacturer to each NIC card. Vendors or manufacturers can use any sequence of digits to the NIC specific digits, but the prefix should be the same as provided by the IEEE. 
 
* The MAC address can be represented in below three formats: 

### Steps to check MAC Address in Microsoft Windows 10 
1. 	Click on Start and search for RUN and open it. 
2.	Type cmd and press ENTER. 
3.	Command Prompt will open, Type ipconfig /all and Press ENTER. 
4.	Under Wireless LAN Adapter, name and physical/MAC address of the device is available. 

---
