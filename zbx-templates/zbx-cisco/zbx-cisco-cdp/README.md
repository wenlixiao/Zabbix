ZBX-CISCO-CDP
==============

This template use the CISCO-CDP-MIB to discover and manage CDP neighbors on Cisco devices.

Items
-----

  * Discovery: CDP neighbor on each interface
  * Discovery: CDP neighbor platform on each interface

Triggers
--------

  * **[INFORMATION]** => Discovery: CDP neighbor on a particular interface was changed.

Installation
------------

1. Install [`advsnmp.discovery`](https://github.com/simonkowallik/Zabbix-Addons/tree/master/advsnmp.discovery) in the **ExternalScripts** directory of your Zabbix server and/or proxy. Check your `zabbix_server.conf` and/or `zabbix_proxy.conf` if in doubt.
2. Then `chmod a+x advsnmp.discovery`
4. Import **zbx-cisco-cdp.xml** file into Zabbix.
5. Add to your host the **{$SNMP_COMMUNITY}** macro with your SNMP community as value.
6. Associate **ZBX-CISCO-CDP** template to the host.
 
### Requirements

This template was tested for Zabbix 2.0.0 or higher.

###### [advsnmp.discovery](https://github.com/simonkowallik/Zabbix-Addons/tree/master/advsnmp.discovery) 2.0

This template use this script as an alternative to the build-in SNMP low level discovery of Zabbix.

License
-------

This template is distributed under the terms of the GNU General Public License as published by the Free Software Foundation; either version 2 of the License, or (at your option) any later version.

### Copyright

  Copyright (c) Jean-Jacques Martrès

### Authors
  
  Jean-Jacques Martrès
  (jjmartres |at| gmail |dot| com)
