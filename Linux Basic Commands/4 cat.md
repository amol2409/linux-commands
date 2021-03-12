# cat

**cat command :** This has 3 related functions regarding text files.
1.  Displaying text files
    
1. Combining text files
    
1. Creating new text files

* **cat :** for echoing, whatever we will type after it will again display on terminal again. To exit this mode press <kbd> ctrl</kbd> + <kbd> D</kbd>.
    
* **cat [filename] :** Show the content of file on terminal.
    
* **cat [filename 1] [filename 2]:** Show the content of 2 files.
    
    <!-- * **cat :** -->

* **cat -n [filename] :** Show file content with line numbers (blank lines also have numbers).

* **cat -b [filename] :** Show file content with line numbers (blank lines don't  have numbers).

* **cat -s [filename] :** If there are more than one blank line then it will remove.

* **cat -E [filename] :** Add $ at the end each line.

* **cat > out.txt :** Whatever you will write on terminal that will be redirected to the file out.txt. If file isn't there then it will create the file and if file exist will replace the old data.

* **cat >> out.txt :**  This will append the data with  old data.