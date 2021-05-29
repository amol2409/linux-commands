# mkdir command

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
