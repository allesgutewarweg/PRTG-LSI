PRTG Device Templates
======================

PRTG Network monitor can create devices and sensors using templates for any device.
The template files identifies devices by matching checks to what's expected by a device type.


[Creating PRTG Device Templates](https://www.paessler.com/manuals/prtg/create_device_template)
[Creating PRTG Custom Scripts](https://kb.paessler.com/en/topic/71356-guide-for-powershell-based-custom-sensors)
--------------------------------
Once you have a device configured with all the sensors you want for that type, 
PRTG can create a base device template for you. Simply select the device and select "Create Device Template" from the menu.

PRTG Device Templates
Installation Instructions
=========================

The template project has a standard directory structure:
All the files in the PRTG subdirectory needs to go into the PRTG program directory
(https://kb.paessler.com/en/topic/463-how-and-where-does-prtg-store-its-data).
The other files are for documentation and testing.
<pre>
 ProjectN_name
   + - traces		      (files to use for testing, SNMP traces etc.)
   + - PRTG               (hierarchy that goes into the PRTG directory)
        + - Custom Sensors	 (Where PRTG stores Custom senosrs)
        + - devicetemplates  (Where PRTG stores the device templates)
        + - lookups          (Where PRTG stores the lookups)
            + - custom       (Where PRTG stores custom lookups)
        + - MIB              (Where PRTG stores MIBs)
        + - notifications	 (Where PRTG stores Custom Notifications)
        + - snmplibs         (Where PRTG stores imported custom OID Libraries)
        + - webroot          (PRTG webgui)
            + - icons        (PRTG webgui icons)
                + - devices  (PRTG device icons)
</pre>

Files to include
================

Custom Sensors
-------------------------
PRTG Custom Sensor  files.

devicetemplates (xxx.odt) 
-------------------------
PRTG device template files.

lookups\custom (xxx.ovl) 
-------------------------
PRTG lookup files for use with sensors with lookup values

lookups\custom (xxx.ovl) 
-------------------------

notifications
-------------------------
Custom PRTG Notifications.

MIB
---
Manufacturer supplied MIB files to include. These will be loaded into PRTG on startup.

snmplibs (xxx.oidlib)
---------------------
Files imported from MIB files by the [Paessler MIB importer](https://www.paessler.com/tools/mibimporter).

webroot\icons\devices (vendors_xxx.png)
---------------------
Icon files used by PRTG to display in the tree. Should be 14.14 pixel PNG's.



