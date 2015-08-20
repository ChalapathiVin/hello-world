hello-world
===========

First repository

SCCM:
-A single collection can contain users or devices, but not both.

-Do not use incremental updates for large number of collections [Incremental updates occur at 10 minute interval. Independently of a full collection evaluation]

-Schedule a full update on this collection :to schedule a regular full evaluation of the collection membership. The members will not appear in the collection until after the first scheduled update, or you manually select Update Membership for the collection. 

-If a collection includes both include collection and exclude collection rules and there is a conflict, the exclude   collection rule takes priority over the include collection rule.

-Operating System Name and Version
  Workstation 6.1 – Windows 7
  Workstation 6.2 – Windows 8
  Server 6.1 – Windows Server 2008 R2
  Server 6.2 – Windows Server 2012
 [SMS_R_System.OperatingSystemNameandVersion like "%Workstation 6.1%"]

-SMS_R_System.NetbiosName

-Device types are stored in the Configuration Manager database under the resource class sms_r_system and the attribute  name AgentEdition. SMS_R_System.ClientEdition = 5 [mac comps]

-Direct Membership Rule Wizard
 *Resource class:Select from "System Resource" values to search for inventory data returned from client computers or   "Unknown  Computer" to select from values returned by unknown computers.
 *Exclude resources marked as obsolete
 *Exclude resources that do not have the Configuration Manager client installed

-Query Rule Properties
 *Import Query Statement
 *Resource class
