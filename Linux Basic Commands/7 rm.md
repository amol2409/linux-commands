# rm command

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
