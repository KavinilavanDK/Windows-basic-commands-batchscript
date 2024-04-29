## NAME:KAVI NILAVAN DK
## REG NO:212223230103


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
![01](https://github.com/KavinilavanDK/Windows-basic-commands-batchscript/assets/144870429/71b0ec7e-cbd3-458f-a67b-50ea520aa5b3)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```
![02](https://github.com/KavinilavanDK/Windows-basic-commands-batchscript/assets/144870429/7ce239b8-8187-470c-a7ac-eb9d97228257)


![03](https://github.com/KavinilavanDK/Windows-basic-commands-batchscript/assets/144870429/2d364284-f23c-4bde-8071-d98bb55bb590)

List the contents of the "MyLab" directory.
## COMMAND AND OUTPUT
```
dir %userprofile%\Desktop\MyLab
```
![04](https://github.com/KavinilavanDK/Windows-basic-commands-batchscript/assets/144870429/e661a2ff-a556-4d69-a2bb-69a8eb6ac7c3)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```
![05](https://github.com/KavinilavanDK/Windows-basic-commands-batchscript/assets/144870429/68966b86-191c-40ee-957e-d1f5fa36d786)

![06](https://github.com/KavinilavanDK/Windows-basic-commands-batchscript/assets/144870429/d0e46ae6-fb3b-4181-bf8d-18ad0b747558)

Move the "MyLab" directory to the "Documents" folder.

## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```

![08](https://github.com/KavinilavanDK/Windows-basic-commands-batchscript/assets/144870429/1320f93b-9ca4-45a6-b03f-f8e6030f3145)


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
![07](https://github.com/KavinilavanDK/Windows-basic-commands-batchscript/assets/144870429/873a461c-c805-4108-974d-374bb6984f97)

# RESULT:
The commands/batch files are executed successfully.

