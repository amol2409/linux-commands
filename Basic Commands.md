# Basic Commands

* Few Basic Commands are as follows

## pwd  

This will show the present working directory, you are working on.

## ls

* This will list the files in present working directory. This can be use in many ways:
 **Syntax :** **ls [options] [directory path]**

1. **ls .. :** List files in parent directory.

2. **ls ../.. :** List files in grand parent directory.

3. **ls ~:** List the files of home directory.

4. **ls -a :** list all files with all hidden files. Usually files and folders started with . or .. are hidden files and folders.

* **ls -A :** This will show all hidden files and folders except . and ..

* **ls -l :** List all the files with all information.

* **ls -S :** This will order the files and folders in descending order of their size but did not show the size. In order to show the size use **ls -lS**.

* **ls -d :** list all directory only.

* **ls** ***.html :** list all html files.

* **ls** ***.*** **:** list all files.

* **ls -R :** See the directory structure.

* **ls -al > out.txt :** This will write the the all files and folder info into out.txt file.

## cd

**cd command :** This is used to change the directory in following ways.

1. **cd :** Change to home directory.

2. **cd ~ :** Change to home directory.
        * actually **~** is equal to  **/home/amol**

3. **cd / :** Change to root directory.

4. **cd .. :** Change to parent directory.
5. **cd [path] :** Path can be absolute or relative.
6. **cd AP ES :** AP ES is the folder name with space. In this case command will not run. In order to fix it use cd command in following way.
  
* **cd AP\ ES :** With back slash
* **cd "AP ES" :**
* **cd 'AP ES' :**

## cat

**cat command :** This has 3 related functions regarding text files.

1. Displaying text files
2. Combining text files
3. Creating new text files

* **cat :** for echoing, whatever we will type after it will again display on terminal again. To exit this mode press  "ctrl +  D".

* **cat [filename] :** Show the content of file on terminal.
* **cat [filename 1] [filename 2]:** Show the content of 2 files.
* **cat -n [filename] :** Show file content with line numbers (blank lines also have numbers).
* **cat -b [filename] :** Show file content with line numbers (blank lines don't  have numbers).
* **cat -s [filename] :** If there are more than one blank line then it will remove.
* **cat -E [filename] :** Add $ at the end each line.
* **cat > out.txt :** Whatever you will write on terminal that will be redirected to the file out.txt. If file isn't there then it will create the file and if file exist will replace the old data.
* **cat >> out.txt :**  This will append the data with  old data.

## mkdir command

* This command is used to create directories.

**syntax:** mkdir [options]... [directories name]

**Options:**

1. **-p or --parents :** This option will create parent directory if needed.
2. **-v or --verbose :** Print a message for each directory created.

**Examples:**

1. **mkdir temp :** Create temp folder.
2. **mkdir temp/test :** Create test folder inside temp. temp must be existed before executing this command.
3. **mkdir -p abc/def :** If abc and def not existed before then using **-p** option we can create this.
4. **mkdir -p number/{real,rational,integer} :** This will create a number directory which has 3 more directory in it (real,rational,integer).
5. **mkdir -v number :** This will create temp directory and display message like "**mkdir: created directory 'number'**"

**eg.** Create directory structure like **a/b/c/d/e/f/g**

```bash
    mkdir -p a/b/c/d/e/f/g
```

## rmdir command

This command is used to remove empty directories or empty directory structure.

**Syntax :** rmidr [options...] [directory name...]

**Options:**

1. **-p or --parents :** This option will remove all directory structure
2. **-v or --verbose :** Print a message for each directory removed.

**eg.**

``` bash
    # This will create directory structure
    mkdir -p a/b/c/d/e
    
    # This will remove only top level directory which is e
    rmdir a/b/c/d/e 

    # In order to remove entire directory structure use -p option
    rmdir -p a/b/c/d/e
```

## rm command

* This command is used to remove directories and files.

**Syntax :** rm [options...] [directory name...] [Files...]

**Options :**

1. **-r or -R or --recursive:** To delete a directory or directory structure we have to give this option.
2. **-v or --verbose :** Print a message for each directory removed.
3. **-f :** forcing to delete without prompt.

**Examples :**

**eg1.** To delete files.

``` bash
    touch test.cpp temp.cpp
    rm test.cpp temp.cpp
```

**eg2.** To delete directories.

``` bash
    mkdir -p a/b/c/d/e
    rm -r a
```

**eg3.** To delete all files in a directory.

``` bash
    rm *
```

## cp command

* This command is use to copy the data from source to destination.

**Syntax :** cp [options] [source] [destination]
**Note :**

1. **Source :** Source can be single file or multiple files or single directory or multiple directory.
1. **Destination :** Destination can be either single file or single directory.

1. **Flow :**
    * single source file --> destination file
    * multiple source file --> destination folder
    * single source folder --> destination folder
    * multiple source folder --> destination folder

**Examples  :**

1. **file to file copy:**
    **Example :**
    * **cp file1.txt file2.txt :** This will copy the data of file1 into file2. (If file2 doesn't exist then it will create file2).

    * **cp /home/amol/Documents/file1.txt /home/amol/Desktop/file2.txt :** This will copy file1 from documents folder to file2 of Desktop folder. (If file2 doesn't exist then it will create file2).

1. **multiple files to directory :**
    **Example:**
    * **cp f1.txt f2.txt ~/Desktop :** Copy f1 and f2 into Desktop directory.

1. **dir to dir :** for this we usually use **-r** as an option.
    **Example :**
    * **cp -r dir1 dir2 :** Copy dir1  to dir2

1. **Multiple dir to dir :**
    **Example :**
    * **cp -r dir1 dir2 dir3 :** Copy dir1 dir2 to dir3. (If dir3 doesn't exist then dir3 will be created.)

## mv command

* This command is used to move the files and folders. If we are moving in the same dir then that's renaming.

**Syntax :** mv [options...] [Source] [Destination]

**Options :**

1. **-i :** This will prompt before overwrite a file. press y and enter will overwrite and press n and enter will not overwrite.

2. **-v or --verbose :** Print a message for each directory removed.

**Renaming :**

``` bash
    touch add.cpp
    # This mv command rename the add.cpp to sub.cpp
    mv add.cpp sub.cpp

    mkdir add
    # This mv command rename add directory to sub
    mv add sub
```

## less command

* Less command is used to display text file on terminal or output of a other command on terminal. If we open a file using some editor than entire file will open. But less command will not open entire file. This command open text file page by page.
* This is mostly used to open big files.

**Syntax :** *less [options...] fileName*

There are many option in this command. In order to go through all options just press ***h***.

**Examples :**

## touch command

Touch is used to create empty files and changing the timestamps of existed files.

**Syntax :** *touch [option...] fileName*

**Create New File :**

``` bash
    touch temp.txt
```

**Create Multiple File :**

``` bash
    touch file1 file2 file3
```

**Don't wana create :** Using *-c* we will stop touch utility to create new file. If file is already exist then it will change timestamps of file.

``` bash
    touch -c test.cpp
```

### Linux Files Timestamps

A file in linux has three timestamps.

1. **Access Time :** The last time file was accessed or opened by some command or application like vim, cat, grep.

1. **Modify Time :** The last time file content was modified.

1. **Change Time :** The last time the file’s attribute or content was changed. The attribute includes file permissions, file ownership or file location.

**Note :** In order to see the timestamps or other info use ***stat*** command.

``` bash
    stat filename
```

**Example for timestamp change :**
If we don't use any option then all timestamps will change for existed file.

``` bash
    # Assume test is already created then below command
    # will change all timestamps
    touch test

    # only access time will change
    touch -a test

    # only change and modify time will change
    touch -m test
```

**Questions :** All of these examples will work with ***mkdir*** also.

**Q:1** Create 9 files test1 test2 and test9

``` bash
    touch test{1,2,3,4,5,6,7,8,9}
```

**Q2:** Create 9 test files like test1.cpp test2.cpp test3.cpp...

``` bash
    touch test{1,2,3,4,5,6,7,8,9}.cpp
```

**Q3:** Create  file like amol-gate, sid-gate, amol-net, sid-net, amol-jre, sid-jre

``` bash
    touch {amol,sid}-{gate,net,jre}
```

**Q4:** Create files like a1,a2,..a5   b1,b2..b5 .... e1,e2...e5

``` bash
    touch {a..e}{1..5}
```
