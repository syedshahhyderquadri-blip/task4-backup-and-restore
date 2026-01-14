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


<img width="1084" height="705" alt="Image" src="https://github.com/user-attachments/assets/4a7c8df3-a8dd-4f3a-8389-a8b8b8ce04a3" />

<img width="1576" height="212" alt="Image" src="https://github.com/user-attachments/assets/024613f9-59f5-4c68-94e4-3074148cc63b" />

<img width="1142" height="189" alt="Image" src="https://github.com/user-attachments/assets/6bc4e712-a287-4026-855e-e855e4566e72" />

<img width="1275" height="388" alt="Image" src="https://github.com/user-attachments/assets/977d15c7-ae0d-4dbe-a188-aa2383e96909" />

<img width="1511" height="80" alt="Image" src="https://github.com/user-attachments/assets/b35d0814-93c5-4e1b-bcaa-7ca1773d3b8d" />

<img width="1092" height="77" alt="Image" src="https://github.com/user-attachments/assets/80f08860-8ad4-4ea4-b511-346f8225589e" />

<img width="1008" height="962" alt="Image" src="https://github.com/user-attachments/assets/43ae89f8-01de-41cf-b7d2-d6c3e7db9873" />

<img width="1172" height="374" alt="Image" src="https://github.com/user-attachments/assets/ac2d1a91-867b-4895-9e7b-8fda63d1fa63" />



