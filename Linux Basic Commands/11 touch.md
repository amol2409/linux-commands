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
