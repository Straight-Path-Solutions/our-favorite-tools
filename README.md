# Our favorite FREE community supported SQL Server scripts (that we didn’t make)

As you may have noticed, here at [Straight Path Solutions](https://straightpathsql.com/) we’ve been working on a few free scripts to help you with maintaining your SQL Server instances. These include:<br>
  •	[sp_CheckBackup](https://github.com/Straight-Path-Solutions/sp_CheckBackup) to reveal the history and problems with your database backups<br>
  •	[sp_CheckSecurity](https://github.com/Straight-Path-Solutions/sp_CheckSecurity) to uncover security vulnerabilities with your instance<br>
  •	[sp_CheckTempdb](https://github.com/Straight-Path-Solutions/sp_CheckTempdb) to get the configuration and any issues with your tempdb database<br>
<br>
<br>
However, we also want to draw attention to the scripts created by other folks that we use nearly every day. Whether you are just starting with SQL Server or have been working with databases for decades, it’s very likely you could benefit from one or more of these scripts.
<br>
We’ve made this page on our GitHub repo to share these scripts for any folks that happen upon the repo, but since you’re here...here’s what we often use!<br>
<br>

# Adam Machanic’s sp_WhoIsActive

Adam Machanic’s [sp_WhoIsActive](https://github.com/amachanic/sp_whoisactive) is probably the most frequently used community tools of all time. And that’s with good reason, since it tells you a whole lot of information about what is happening RIGHT NOW on your SQL Server instance. It also has many useful parameters for helping to filter and collect this data.<br>
<br>

# Ola Hallengren’s Maintenance Solution

[Ola Hallengren’s Maintenance Solution](https://ola.hallengren.com/) has been the gold standard for SQL Server database maintenance scripts and jobs for over a decade. [We even have a handy blog post](https://straightpathsql.com/archives/2023/01/ola-maintenance-from-a-jr-dba/) about this. Ola’s solution includes:<br>
  •	[DatabaseBackup](https://github.com/olahallengren/sql-server-maintenance-solution/blob/main/DatabaseBackup.sql) for backing up SQL Server databases in a zillion ways to nearly any kind or destination.<br>
  •	[DatabaseIntegrityCheck](https://github.com/olahallengren/sql-server-maintenance-solution/blob/main/DatabaseIntegrityCheck.sql) for checking for corruption and consistency errors.<br>
  •	[IndexOptimize](https://github.com/olahallengren/sql-server-maintenance-solution/blob/main/IndexOptimize.sql) for regularly scheduled index maintenance (TIP: you probably shouldn’t use the defaults since they may result in a lot of extra activity that might be more harmful than helpful.)<br>
  •	A helpful CommandLog table to collect execution information.<br>
<br>

# Brent Ozar’s First Responder Kit

[Brent Ozar’s First Responder Kit](https://github.com/BrentOzarULTD/SQL-Server-First-Responder-Kit) is known for [sp_Blitz](https://github.com/BrentOzarULTD/SQL-Server-First-Responder-Kit?tab=readme-ov-file#sp_blitz-overall-health-check), which is great for quickly collecting a ton of information about the overall health of a SQL Server instance with helpful links to content about any findings, but there are other wonderful scripts including:<br>
  •	[sp_BlitzCache](https://github.com/BrentOzarULTD/SQL-Server-First-Responder-Kit?tab=readme-ov-file#sp_blitzcache-find-the-most-resource-intensive-queries) looks at your plan cache and helps find the most resource-intensive queries<br>
  •	[sp_BlitzIndex](https://github.com/BrentOzarULTD/SQL-Server-First-Responder-Kit?tab=readme-ov-file#sp_blitzindex-tune-your-indexes) is an indispensable tool for tuning indexes.<br>
  •	[sp_BlitzLock](https://github.com/BrentOzarULTD/SQL-Server-First-Responder-Kit?tab=readme-ov-file#sp_blitzlock-deadlock-analysis) parses the XML of the System Health extended event and presents deadlock info you can read.<br>
  •	[sp_DatabaseRestore](https://github.com/BrentOzarULTD/SQL-Server-First-Responder-Kit?tab=readme-ov-file#sp_databaserestore-easier-multi-file-restores) is the easiest way to restore databases backed up with Ola Hallengren’s DatabaseBackup.<br>
  •	[sp_ineachdb](https://github.com/BrentOzarULTD/SQL-Server-First-Responder-Kit/blob/dev/sp_ineachdb.sql) is a fully featured alternative to the undocumented and sometimes unreliable sp_msforeachdb.<br>
<br>

# Erik Darling’s Troubleshooting Scripts

[Erik Darling’s Troubleshooting Scripts](https://github.com/erikdarlingdata/DarlingData) that include:<br>
  •	[sp_HumanEvents](https://github.com/erikdarlingdata/DarlingData/tree/main/sp_HumanEvents) allows you to easily use Extended Events to track common query issues like Blocking.<br>
  •	[sp_HumanEventsBlockViewer](https://github.com/erikdarlingdata/DarlingData/tree/main/sp_HumanEvents) helps with reading the XML output of the “blocked process report” Extended Event.<br>
  •	[sp_QuickieStore](https://github.com/erikdarlingdata/DarlingData/tree/main/sp_QuickieStore) allows you to dig into Query Store beyond the built-in reports.<br>
  •	[sp_PressureDetector](https://github.com/erikdarlingdata/DarlingData/tree/main/sp_PressureDetector) is a fantastic tool for detecting memory and CPU pressure.<br>
<br>

# Andy Yun’s sp_helpExpandView

Andy Yun’s [sp_helpExpandView](https://github.com/SQLBek/sp_helpExpandView) helps make sense of any gross nested views.<br>
<br>

# Glenn Alan Berry’s SQL Server Diagnostic Queries

Glenn Alan Berry’s [SQL Server Diagnostic Queries](https://glennsqlperformance.com/resources/) are great to review your SQL Server instance. Glenn has regularly updated scripts for versions back to SQL Server 2005, and includes result spreadsheets, Jupyter Notebooks, and a training video to get you started quickly.<br>
<br>

# dbatools

And finally, these aren’t T-SQL scripts, but if you manage SQL Server anywhere then you we highly recommend you get at least a little familiar with PowerShell and explore the hundreds of cmdlets at [dbatools.io](https://dbatools.io/). It will make your life so much easier!
