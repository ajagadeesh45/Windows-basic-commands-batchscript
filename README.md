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
```c
mkdir %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/9115620f-1a86-4a2b-ae53-f0e1d26b359f)



Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
```c
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/ebd91539-0e28-43c6-9e87-ebb3f6e128c7)
```c
type nul > MyFile.txt
```
![image](https://github.com/user-attachments/assets/869ca1ca-0bd7-43c0-880f-370cc4c12092)



List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
```c
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/66e8c7bd-bab0-444c-8fd8-95fdcf3a71a6)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
```c
mkdir %userprofile%\Desktop\Backup
```
![image](https://github.com/user-attachments/assets/1b776f5d-2080-4771-8ba4-bf3bbe7ac7e0)
```c
copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/user-attachments/assets/85d89d2c-6fcb-496c-b7ac-b9a2793122ca)





Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
```c
mkdir %userprofile%\Desktop\Documents
```
![image](https://github.com/user-attachments/assets/5a779f09-d4eb-499e-8476-7a7cb18015aa)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
# COMMAND
```c
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```








## OUTPUT
![image](https://github.com/user-attachments/assets/35d59cb9-4e09-468f-9c2a-78e990509a63)






# RESULT:
The commands/batch files are executed successfully.

