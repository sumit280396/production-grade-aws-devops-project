# What docker actually is in Linux 

- Docker actually runs as a daemon(process) in Linux

## Daemon
- Daemon is a program which runs in the background, does not need any inputs and no outputs on the screen and wakes up and do tasks when their trigger arises(example- ngnix is a daemon which waits for http requests)
- Daemon processes are started by the PID 1 process which is **systemd** during the boot

### How to check for all the processes in Linux?
``` ps -e ```
``` ps aux ``` - This command gives the detailed output of all the processes

### How to identify which processes are the daemon processes?
- The processes under which the **TTY** is **?**, those are the daemon processes
- **TTY** means the process does not have any terminal or screen to output on
