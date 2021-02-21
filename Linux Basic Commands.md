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

1. **mkdir command :**

    







