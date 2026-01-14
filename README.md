# task4-backup-and-restore


COMPANY: CODETECH IT SOLUTUIONS PRIVATE LIMITED 

NAME:SYED SHAH HYDER QUADRI

INTERN ID: A42D0A63D4B671FF

DOMAIN:SQL

DURATION:4 WEEKS

MENTOR:NEELA SANTOSH 


# Task 4: Oracle Database Backup & Restore

## Steps:

1. Create a folder in Windows:
   - Path: C:\oracle_backup

2. Open SQL Command Line (SQL*Plus) and connect:
   - Command: sqlplus system/12345@XE

3. Create Oracle directory:
   ```sql
   CREATE OR REPLACE DIRECTORY backup_dir AS 'C:\oracle_backup';

4.Take database backup (CMD):
expdp system/12345@XE directory=backup_dir dumpfile=oracle_backup.dmp logfile=oracle_backup.log

5.Check that backup files exist in C:\oracle_backup:

6.Restore database (CMD):
impdp system/12345@XE directory=backup_dir dumpfile=oracle_backup.dmp logfile=restore.log

7.Verify tables in SQL*Plus:
SELECT table_name FROM user_tables;



OUTPUTS 



