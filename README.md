```K S Ashwin Kumar```
```212224040034```


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

![image](https://github.com/user-attachments/assets/792d3d77-2adb-4099-b769-41564d837d6d)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/ff82bb4b-6810-49f4-95f7-1f16a1bd5116)


```
type nul > MyFile.txt
```
![image](https://github.com/user-attachments/assets/765a8a03-aea2-4a38-af3e-fe79211c9abd)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
```
dir %userprofile%\Desktop\MyLab
```

![image](https://github.com/user-attachments/assets/6bae0a39-c3a8-43d0-b4b9-da5cf395acd5)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup
```
![image](https://github.com/user-attachments/assets/7c7b17e8-cff3-41e0-9d09-a75c669511be)

```
copy MyFile.txt %userprofile%\Desktop\Backup`
```

![image](https://github.com/user-attachments/assets/ea31b5e4-edae-4f4c-be0b-a8a7f3bd3778)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Documents
move MyLab Documents
```

![image](https://github.com/user-attachments/assets/3f34c0a1-a0dd-43d2-a5ea-de2ffd675792)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

COMMAND:
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```

## OUTPUT
![image](https://github.com/user-attachments/assets/507e511f-00ed-4aa4-9173-8a7f8914d8ea)


# RESULT:
The commands/batch files are executed successfully.

