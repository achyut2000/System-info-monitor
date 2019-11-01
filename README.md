# System-info-monitor
Shell Script to monitor system information.

# Description 

Are you not bored of using the builtin task manager to look of your system.
This is the only reason for creating this project.
This project gets all the info of your system using a **dmidecode** command and some files in your root directory.


# dmidecode 
  is a tool for dumping a computer's DMI (some say SMBIOS ) table contents in a human-readable format. This table contains a description of the system's hardware components, as well as other useful pieces of information such as serial numbers and BIOS revision.
 
- Using text sculpting tools like sed, grep and awk we scrapped the internal files and dmidecode command and printed in a human readable and managable manner.

# Code Details
  - Hardware info
  - ARP info
  - Routing Table
  - OS
  - CPU Usage
  - CPU monitoring
  - Memory usage
  - CPU top 10 processess
  - MEMORY top 10 processess
  - Files used
  - Traffic (Packets)
  
# Usage
```
  > sudo [filename].sh 
    -> gives list of commands to use.
    -> output will be
    Usage : sudo filename [item]
	      item list
	      -----------
	      hardware
	      arp
	      route
	      os
	      cpu
	      cpu_monit
	      mem
	      ctop
	      mtop
	      fileuse
	      traffic
    >sudo filename hardware
      -> gives hardware information
      -> similarly all the commands gives respective information
  ```
# Files used
 - **/sbin/arp**                    -- for arp info
 - **/sbin/route**                  -- for routing table
 - **/etc/issue and /proc/version** -- for os version
 - **/proc/stat**                   -- for cpu stats
 - **/proc/meminfo**                -- for memory info
 - **/proc/sys/fs/file-nr**         -- for file system info
 - **/proc/net/dev**                -- for traffic(packets)
