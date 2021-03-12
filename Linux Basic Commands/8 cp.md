# cp command
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
