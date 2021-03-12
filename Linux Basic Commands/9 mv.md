# mv command
This command is used to move the files and folders. If we are moving in the same dir then that's renaming.

**Syntax :** mv [options...] [Source] [Destination]

**Options :**
1.  **-i :** This will prompt before overwrite a file. press y and enter will overwrite and press n and enter will not overwrite.

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

