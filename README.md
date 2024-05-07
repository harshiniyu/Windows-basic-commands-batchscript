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
mkdir %userprofile%\Desktop\MyLab
![image](https://github.com/harshiniyu/Windows-basic-commands-batchscript/assets/144979786/96d26afe-dff4-4c5a-b317-c05f6c8b1ba7)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab
![image](https://github.com/harshiniyu/Windows-basic-commands-batchscript/assets/144979786/5f886d97-a185-4e5d-9eda-688d599a9c38)

![image](https://github.com/harshiniyu/Windows-basic-commands-batchscript/assets/144979786/568a1af5-cd29-4a05-920f-03e1ff743646)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
copy MyFile.txt %userprofile%\Desktop\Backup
![image](https://github.com/harshiniyu/Windows-basic-commands-batchscript/assets/144979786/80d5c003-96fb-48ee-a71d-cce202d05b3f)

![image](https://github.com/harshiniyu/Windows-basic-commands-batchscript/assets/144979786/8d4410a4-faac-4b72-90c1-424bf84e8da6)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents
![image](https://github.com/harshiniyu/Windows-basic-commands-batchscript/assets/144979786/714260b2-229a-42d3-badb-56ef625e62d7)

![image](https://github.com/harshiniyu/Windows-basic-commands-batchscript/assets/144979786/72114d1d-69f3-4cd6-98ce-1f5ef04502be)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents

![image](https://github.com/harshiniyu/Windows-basic-commands-batchscript/assets/144979786/50e384b7-d0d2-401b-a607-adf46c4c9e77)


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
![image](https://github.com/harshiniyu/Windows-basic-commands-batchscript/assets/144979786/294f3935-f2b1-407a-bb5b-ba4f5737358b)





# RESULT:
The commands/batch files are executed successfully.

