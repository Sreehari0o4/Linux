# Basic Linux Commands

## 1. `ls`
- **Description**: Lists files and directories in the current directory.
- **Usage**: 
  ```bash
  ls
  ls -l     # Long listing format
  ls -a     # Includes hidden file

## 2. `cd`
- **Description**: Changes the current directory.
- **Usage**: 
  ```bash
  cd /path   #path: location of the required directory
  cd /home/user/docs
  cd ..     #go up one level
  cd        #goes to home directory

## 3. `pwd`
- **Description**: Present working directory. It prints the current working directory.
- **Usage**: 
  ```bash
  pwd

## 4. `mkdir`
- **Description**: Creates new directory.
- **Usage**: 
  ```bash
  mkdir dir_name
  mkdir myfolder
  mkdir -p firstdir/secdir # Creates nested directories.

## 5. `touch`
- **Description**: Creates new file.
- **Usage**: 
  ```bash
  touch file_name
  touch file.txt

## 6. `rm`
- **Description**: Remove files or directories.
- **Usage**: 
  ```bash
  rm filename       #removes file
  rm -r foldername  #removes folder
  rm -rf foldername #force delete folder. It deletes non-empty folders.

## 7. `cp`
- **Description**: copies file and directories.
- **Usage**: 
  ```bash
  cp target destination
  cp file1.txt file2.txt    # Copy file1's content to file2
  cp -r dir1/ dir2/         # Copy directory

## 8. `mv`
- **Description**: Moves or renames file or directories.
- **Usage**: 
  ```bash
  mv oldname.txt newname.txt    # rename a file
  mv file.txt /path             # move a file to another folder

## 9. `cat`
- **Description**: displays file content.
- **Usage**: 
  ```bash
  cat file.txt
  cat /path/file.txt

## 10.Path
- A path is a unique location to a file or a folder in a file system of an OS. A path to a file is a combination of / and alpha-numeric characters. 
- Two types: **Absolute** and **Relative**
- **Absolute**:specifying location of file or directory from the root directory(/).
  ```bash
  cd /home/docs/files
  cat /home/devops/commands.txt
- **Relative**:Path related to the present working directory(pwd). Suppose I have multiple folders in current directory and I need to change to one of them I can use relative path. The path that does not start with / diectory.
  ```bash
  cd devopsdir/