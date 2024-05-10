# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file
Save each script in a file with a .bat extension.
Ensure you have the necessary permissions to perform the operations.
Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 

# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\MyLab
```
![image](https://github.com/MALENIMURUGAN/Windows-basic-commands-batchscript/assets/144870675/9cc93d9e-96cb-4bbf-a989-4f668674fa9a)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/MALENIMURUGAN/Windows-basic-commands-batchscript/assets/144870675/e722b054-d488-4215-a9d1-9f20d965a7b4)

![image](https://github.com/MALENIMURUGAN/Windows-basic-commands-batchscript/assets/144870675/2f8936c7-6fed-47e9-8eda-24154d93eb50)

## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/MALENIMURUGAN/Windows-basic-commands-batchscript/assets/144870675/6b4fb369-8069-41dd-b6d7-8be1b092b908)


## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/MALENIMURUGAN/Windows-basic-commands-batchscript/assets/144870675/c7954f05-9519-41e9-903e-5aed3b120491)
![image](https://github.com/MALENIMURUGAN/Windows-basic-commands-batchscript/assets/144870675/3f21759a-00f0-401e-9fce-303d4c675245)


## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![image](https://github.com/MALENIMURUGAN/Windows-basic-commands-batchscript/assets/144870675/2392881d-c4a4-49d8-bf49-ad2c70267377)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
 Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.
 ```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```
## OUTPUT

![image](https://github.com/MALENIMURUGAN/Windows-basic-commands-batchscript/assets/144870675/129249cc-e178-4963-a188-cffd63dc0145)

# RESULT:
The commands/batch files are executed successfully.

