Providing **100 examples of Huawei SAN switch or Brocade SAN switch maintenance commands** could be helpful for varied use cases. Here’s a tabulated list divided into relevant categories for easier navigation.

---

### **1. System Information and Basic Commands**

| **Command**                  | **Description**                                      |
|------------------------------|----------------------------------------------------|
| `switchshow`                 | Displays switch status and details.                |
| `chassisshow`                | Shows chassis-specific information.                |
| `version`                    | Displays firmware version.                         |
| `uptime`                     | Displays system uptime.                            |
| `ipaddrshow`                 | Displays IP address of the switch.                 |
| `fabicshow`                  | Displays all connected switches in the fabric.     |
| `nsallshow`                  | Lists all devices registered in the fabric.        |
| `licenseshow`                | Shows all licenses installed on the switch.        |
| `tempshow`                   | Displays current temperature sensors' data.        |
| `sensor`                     | Displays sensor-related details.                   |

---

### **2. Time Management**

| **Command**                  | **Description**                                      |
|------------------------------|----------------------------------------------------|
| `date`                       | Displays current date and time.                    |
| `tsclockserver`              | Sets or shows NTP server configurations.           |
| `tstimezone`                 | Configures or displays the time zone.              |
| `timesyncstart`              | Manually synchronizes with the NTP server.         |
| `clockset "MM/DD/YYYY HH:MM:SS"` | Manually sets the system clock.               |

---

### **3. Configuration Commands**

| **Command**                  | **Description**                                      |
|------------------------------|----------------------------------------------------|
| `configshow`                 | Displays the switch configuration.                 |
| `configupload`               | Uploads configuration to an external server.       |
| `configdownload`             | Downloads configuration from an external server.   |
| `cfgenable <cfg_name>`       | Enables the specified zoning configuration.        |
| `cfgsave`                    | Saves the current zoning configuration.            |
| `cfgdisable`                 | Disables the current zoning configuration.         |
| `zonecreate`                 | Creates a new zone.                                |
| `zonedelete`                 | Deletes an existing zone.                          |
| `zoneshow`                   | Shows zone configurations.                         |
| `fabriclog --show`           | Displays fabric-related logs.                      |

---

### **4. Port Management**

| **Command**                  | **Description**                                      |
|------------------------------|----------------------------------------------------|
| `portshow <port>`            | Displays information about a specific port.        |
| `portenable <port>`          | Enables the specified port.                        |
| `portdisable <port>`         | Disables the specified port.                       |
| `portstatsshow`              | Displays statistics for all ports.                 |
| `porterrshow`                | Shows errors for all ports.                        |
| `trunkshow`                  | Displays trunk port information.                   |
| `islshow`                    | Shows ISL (Inter-Switch Link) details.             |
| `portcfgspeed`               | Configures port speed.                             |
| `portcfgfillword`            | Configures fill-word settings for a port.          |
| `portname <port>`            | Assigns a name to a specific port.                 |

---

### **5. Diagnostics and Logs**

| **Command**                  | **Description**                                      |
|------------------------------|----------------------------------------------------|
| `diagshow`                   | Displays system diagnostic information.            |
| `supportshow`                | Generates a complete switch diagnostic report.     |
| `errdump`                    | Displays error logs.                               |
| `errclear`                   | Clears the error logs.                             |
| `ping <IP>`                  | Tests connectivity to a specific IP.               |
| `traceroute <IP>`            | Traces the route to a specific IP.                 |
| `logdump`                    | Dumps all log entries to the terminal.             |
| `supportftp`                 | Uploads support logs to an FTP server.             |
| `configshow --all`           | Displays all configurations and details.           |
| `historyshow`                | Shows command execution history.                   |

---

### **6. Performance Monitoring**

| **Command**                  | **Description**                                      |
|------------------------------|----------------------------------------------------|
| `perfshow`                   | Displays performance monitoring status.            |
| `statsclear`                 | Clears all performance statistics.                 |
| `statsshow`                  | Displays general performance statistics.           |
| `fcpstatsshow`               | Shows Fibre Channel Protocol statistics.           |
| `portperfshow`               | Shows real-time performance statistics of ports.   |
| `slotstats`                  | Displays statistics for all slots in a chassis.    |
| `latencyshow`                | Shows port-to-port latency information.            |
| `cpuperfshow`                | Displays CPU performance statistics.               |
| `memshow`                    | Displays memory usage.                             |
| `framebuffshow`              | Shows frame buffer utilization.                    |

---

### **7. Security and User Management**

| **Command**                  | **Description**                                      |
|------------------------------|----------------------------------------------------|
| `userconfig --show`          | Displays user accounts.                            |
| `userconfig --add`           | Adds a new user.                                   |
| `userconfig --delete`        | Deletes an existing user.                          |
| `passwd`                     | Changes the password for the current user.         |
| `secpolicydisplay`           | Displays security policies on the switch.          |
| `authutil`                   | Displays authentication configurations.            |
| `securedisable`              | Disables security settings temporarily.            |
| `lockdown`                   | Enables lockdown mode for additional security.     |
| `auditlog --show`            | Displays the audit log.                            |
| `auditlog --clear`           | Clears the audit log.                              |

---

### **8. Firmware Management**

| **Command**                  | **Description**                                      |
|------------------------------|----------------------------------------------------|
| `firmwareshow`               | Displays the current firmware version.             |
| `firmwaredownload`           | Initiates a firmware upgrade.                      |
| `firmwarecommit`             | Finalizes the firmware upgrade process.            |
| `firmwarecheck`              | Checks firmware compatibility before an upgrade.   |
| `firmwaredownloadstatus`     | Displays the status of an ongoing firmware update. |

---

### **9. Fabric and Topology Commands**

| **Command**                  | **Description**                                      |
|------------------------------|----------------------------------------------------|
| `topologyshow`               | Displays the fabric topology.                      |
| `fabricshow`                 | Displays all switches in the fabric.               |
| `pathinfo`                   | Displays path details between two devices.         |
| `nszoneshow`                 | Shows the Name Server and its zoning information.  |
| `fcrfabricshow`              | Displays Fibre Channel Routing fabric details.     |
| `zoneobjectadd`              | Adds an object to an existing zone.                |
| `zoneshow --detail`          | Displays detailed information about zones.         |

---

### **10. Miscellaneous Commands**

| **Command**                  | **Description**                                      |
|------------------------------|----------------------------------------------------|
| `syslogdipshow`              | Displays Syslog server configurations.             |
| `chassisdipshow`             | Shows DIP switch settings for the chassis.         |
| `snmpconfig --show`          | Displays SNMP configuration.                       |
| `snmpconfig --add`           | Adds a new SNMP configuration.                     |
| `historyclear`               | Clears command history.                            |
| `dnsconfig --show`           | Displays DNS configurations.                       |
| `dnsconfig --add`            | Adds a new DNS server configuration.               |
| `alarms --show`              | Displays active alarms.                            |
| `alarmclear`                 | Clears all alarms.                                 |
| `systemstats`                | Displays overall system statistics.                |

---

Let me know if you'd like examples of a specific set of commands explained in detail!
