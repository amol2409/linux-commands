# rmdir command

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
