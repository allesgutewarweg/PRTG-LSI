Installation Instructions
=========================

The template project has a standard directory structure:
All the files in the PRTG subdirectory needs to go into the PRTG program directory
(https://kb.paessler.com/en/topic/463-how-and-where-does-prtg-store-its-data).
This means, copy the files from "prtg" to "%programfiles(x86)%\PRTG Network Monitor" and the 
files will be copied into the correct locations in the subdirectories. 
Please ** NOTE **, the destination "%programfiles(x86)%" is a "protected path " and requires elevated privileges.
(IE if you copy across the network, the "admin user may not have the correct drive mappings).

If there are any MIB files in the package, they will not be loaded until PRTG is rebooted.
Lookups can be manually re-loaded by using the the Admin Tools page "Setup -> System Administration -> Administrative Tools"
or: https://{Your_PRTG_Server_IP_and_Port}/api/loadlookups.htm

The remaining files are for documentation and testing.


Adding a New template
=======================
Create a new template by creating project under:
https://gitlab.com/PRTG-Projects/Device-Templates
give it a name related to the device manufacturer by Import Project from "Repo URL"
using: "https://gitlab.com/PRTG-Projects/BaseTemplateProject.git".
Please also check the option to "Mirror Repository" so updates to the base project will be included.

