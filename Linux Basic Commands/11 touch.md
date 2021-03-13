# touch command

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