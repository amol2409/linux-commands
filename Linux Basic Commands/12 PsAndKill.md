# Process Management

* A process is an instance of a running program. Whenever we run a shell command or shell script in linux machine then a process will be created.

## ps command

* It will show the current running processes.

### Options for ps

1. **ps**
   * It will show the currently running process.
2. **ps -f**
   * It will show the parent id too.
3. **ps -e**
   * It will show all the running process on linux machine.
4. **ps -H**
   * It will indent the process so that one can know visually that which one is parent and child.
5. **ps -ef | grep *(process_name)***
   * *ps -ef* will list all the processes and those processes go as an input to *grep* command which will filter out specific process based on the process name.

## kill command

* It's used to kill currently running processes.

### Options for kill

1. **kill *(process_id)***
   * It wil kill the process whose PID is given as process id.
2. **kill -9 *(process_id)***
   * It will kill the process forcefully with option -9.
