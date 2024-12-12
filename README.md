# SQL-Data-files


The AdventureWorks databases are sample databases that were originally published by Microsoft to show how to design a SQL Server database using SQL Server 2008. AdventureWorks is the OLTP sample, and AdventureWorksDW is the data warehouse sample.

Database design has progressed since AdventureWorks was first published. For a sample database leveraging more recent features of SQL Server, see WideWorldImporters.

Note that AdventureWorks has not seen any significant changes since the 2012 version. The only differences between the various versions of AdventureWorks are the name of the database and the database compatibility level. To install the AdventureWorks databases with the database compatibility level of your SQL Server instance, you can install from a version-specific backup file or from an install script.

Prerequisites
Filestream must be installed in your SQL Server instance.

Install from a script
The install scripts create the sample database to have the database compatibility of your current version of SQL Server. Each script generates the version-specific information based on your current instance of SQL Server. This means you can use either the AdventureWorks or AdventureWorksDW install script on any version of SQL Server including CTPs, SPs, and interim releases.

Install notes
When installing from a script, the default database name is AdventureWorks or AdventureWorksDW. If you want the version added to the name, edit the database name at the beginning of the script.

The oltp script drops an existing AdventureWorks database, and the data warehouse script drops an existing AdventureWorksDW. If you don't want that to happen, you can update the $(DatabaseName) in the script to a different name, for example AdventureWorks-new.

To install AdventureWorks
Copy the GitHub data files and scripts for AdventureWorks to the C:\Samples\AdventureWorks folder on your local client.
Or, download AdventureWorks-oltp-install-script.zip and extract the zip file to the C:\Samples\AdventureWorks folder.
Open C:\Samples\AdventureWorks\instawdb.sql in SQL Server Management Studio and follow the instructions at the top of the file.
To install AdventureWorksDW
Copy the GitHub data files and scripts for AdventureWorksDW to the C:\Samples\AdventureWorksDW folder on your local client.
Or, download AdventureWorksDW-data-warehouse-install-script.zip and extract the zip file to the C:\Samples\AdventureWorksDW folder.
Open C:\Samples\AdventureWorksDW\instawdbdw.sql in SQL Server Management Studio and follow the instructions at the top of the file.
 
