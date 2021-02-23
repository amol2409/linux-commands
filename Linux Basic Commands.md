# Basic Linux Commands

1. **pwd :** This will show the present working directory, you are working on.

1. **ls [options] [directory path]** ls will list the files in present working directory. This can be use in many ways:

    * **ls .. :** List files in parent directory.

    * **ls ../.. :** List files in grand parent directory. 

    * **ls ~:** List the files of home directory.

    * **ls -a :** list all files with all hidden files. Usually files and folders started with . or .. are hidden files and folders.

    * **ls -A :** This will show all hidden files and folders except . and ..
    
    * **ls -l :** List all the files with all information.
    
    * **ls -S :** This will order the files and folders in descending order of their size but did not show the size. In order to show the size use **ls -lS**.
    
    * **ls -d :** list all directory only.
    
    * **ls** ***.html :** list all html files.
    
    * **ls** * **.** * **:** list all files.
    
    * **ls -al > out.txt :** This will write the the all files and folder info into out.txt file.
    
1. **cd command :** This is used to change the directory in following ways. 

    * **cd :** Change to home directory.
    
    * **cd ~ :** Change to home directory.
        
        * actually **~** is equal to  **/home/amol**
    
    * **cd / :** Change to root directory.
    
    * **cd .. :** Change to parent directory.
    
    * **cd [path] :** Path can be absolute or relative.
    
    * **cd AP ES :** AP ES is the folder name with space. In this case command will not run. In order to fix it use cd command in following way.
        
        * **cd AP\ ES :** With back slash
        
        * **cd "AP ES" :** 
        
        * **cd 'AP ES' :**

1. **cat command :** This has 3 related functions regarding text files.

    
    1. Displaying text files
    
    1. Combining text files
    
    1. Creating new text files

    * **cat :** for echoing, whatever we will type after it will again display on terminal again. To exit this mode press <kbd> ctrl</kbd> + <kbd> D</kbd>.
    
    * **cat [filename] :** Show the content of file on terminal.
    
    * **cat [filename 1] [filename 2]:** Show the content of 2 files.
    
    * **cat :**

    * **cat -n [filename] :** Show file content with line numbers (blank lines also have numbers).

    * **cat -b [filename] :** Show file content with line numbers (blank lines don't  have numbers).

    * **cat -s [filename] :** If there are more than one blank line then it will remove.

    * **cat -E [filename] :** Add $ at the end each line.

    * **cat > out.txt :** Whatever you will write on terminal that will be redirected to the file out.txt. If file isn't there then it will create the file and if file exist will replace the old data.

    * **cat >> out.txt :**  This will append the data with  old data.

## mkdir command
This command is used to create directories.

**syntax:** mkdir [options]... [directories name]

**Options:**
1. **-p or --parents :** This option will create parent directory if needed.
1. **-v or --verbose :** Print a message for each directory created. 

**Examples:**
1. **mkdir temp :** Create temp folder.
2. **mkdir temp/test :** Create test folder inside temp. temp must be existed before executing this command.
3. **mkdir -p abc/def :** If abc and def not existed before then using **-p** option we can create this.
4. **mkdir -p number/{real,rational,integer} :** This will create a number directory which has 3 more directory in it (real,rational,integer).
5. **mkdir -v number :** This will create temp directory and display message like "**mkdir: created directory 'number'**"

## cp command
This command is use to copy the data from source to destination.

**Syntax :** cp [options] [source] [destination]
**Note :**
1.  **Source :** Source can be single file or multiple files or single directory or multiple directory.
1. **Destination :** Destination can be either single file or single directory. 

1. **Flow :**
    *   single source file --> destination file
    *   multiple source file --> destination folder
    *   single source folder --> destination folder
    *   multiple source folder --> destination folder

**Examples  :**

1. **file to file copy:**
    **Example :**
    * **cp file1.txt file2.txt :** This will copy the data of file1 into file2. (If file2 doesn't exist then it will create file2).

    * **cp /home/amol/Documents/file1.txt /home/amol/Desktop/file2.txt :** This will copy file1 from doucments folder to file2 of Desktop folder. (If file2 doesn't exist then it will create file2).

1.  **multiple files to directory :**
    **Example:**
    *   **cp f1.txt f2.txt ~/Desktop :** Copy f1 and f2 into Desktop directory.

1. **dir to dir :** for this we usually use **-r** as an option.
    **Example :**
    * **cp -r dir1 dir2 :** Copy dir1  to dir2

1. **Multiple dir to dir :**
    **Example :**
    * **cp -r dir1 dir2 dir3 :** Copy dir1 dir2 to dir3. (If dir3 doesn't exist then dir3 will be created.)









