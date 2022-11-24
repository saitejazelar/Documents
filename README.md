# Azure DevOps Server On-Prem installation Requirements


* Latest Version of Azure DevOps Server is 2022

* Azure DevOps Server can be installed on a Single Server or Multiple Servers.


## Installation on a Single Server:

The Hardware Requirements for the servers are based on the size of the team.

Upto 250 users the hardware requirements are:
➢	one dual-core processor
➢	4GB RAM
➢	Fast HDD

●	Upto 500 users the hardware requirements are:
➢	Two dual-core processors if elastic search feature is needed
➢	8GB RAM
➢	Fast HDD

●	If Azure DevOps Server is Installing on Server Operating System the supported OS are:
➢	For Azure DevOps Server 2022 the supported server OS are windows 2022 & windows 2019
➢	For Azure DevOps Server 2020 the supported server OS windows 2019 & windows 2016

●	If Azure DevOps Server is Installing on Client Operating System the supported OS are:
➢	For Azure DevOps Server 2022 the supported client OS are windows 11 version 21H2 & windows 10 1809 or later
➢	For Azure DevOps Server 2020 the supported client OS are windows 10 Enterprise version 21H2 & windows 10 1809 or later

➔	 Azure SQL Database and SQL Server:

➢	Azure DevOps on-premises deployments require some version of SQL Server. Azure DevOps Server supports Express, Standard, and Enterprise
➢	The Express edition is recommended only for evaluation purposes, personal use, or for very small teams. We recommend the SQL Server Standard or Enterprise versions for all other scenarios.


➢	 The account you use to configure the installation must be a member of the sysadmin server role in SQL Server.

Note:
	Installing Azure DevOps on-premises involves a complex set of operations 	that 	require a high degree of privilege. These operations include creating 	databases, 	provisioning logins for service accounts, and more. Technically, all that's required 	is:
•	  Membership in the serveradmin role.
•	  ALTER ANY LOGIN, CREATE ANY DATABASE, and VIEW ANY 		 	 DEFINITION server-scoped permissions.
•	  DEFINITION server-scoped permissions.
•	  CONTROL permission on the master database.
Membership in the sysadmin server role confers all these memberships and permissions. It's the easiest way to ensure that configuration succeeds. If necessary, you can revoke these memberships and permissions after installation.

➔	Installation on a Multiple Servers:

➢	The following scenarios might require a multiple-server deployment:

The following scenarios might require a multiple-server deployment:

●	Scaling beyond 500 users
●	Extensive use of automated build, test, or release
●	Using Code Search
●	Using reporting features

➢	For a team of more than 500 users, consider the following setup:
➢	An application tier with one dual-core processor, 8 GB of memory, and a fast hard-disk drive.
➢	A data tier with one quad-core processor, 16 GB of memory, and high-performance storage, such as an SSD.

        
➢	For a team of more than 2,000 users, consider the following setup:
•	An application tier with one quad-core processor, 16 GB or more of memory, and a fast hard-disk drive.
•	A data tier with two or more quad-core processors, 16 GB or more of memory, and advanced high-performance storage, like an SSD or high-performance SAN.
•	If you plan to use build, test, or release automation extensively, we recommend that you use higher-spec application and data tiers to avoid performance issues.
