# Core components of Linux :
- Hardware :
The physical component where OS is installed.
- Kernel :
The heart of Linux. The central core that directly controls hardware, processes, memory. Interface between hardware and software. Machine understands kernel language.
- Shell :
Interactive way to talk to kernel using commands.
- GUI :
Graphical user interface for visual interaction.
- System Libraries : 
Collections of pre-written functions that applications use to request services from the kernel.
- System Utilities : 
Programs and tools (like ls, cp, grep) that perform specific tasks, managing files, users, and system operations.

# Processes in Linux
Processes are instances of running programs. For ex. if you do pin ww.google.com then ping process is created.
You can list processes using ps(ps ax, ps ef) or top commands. 
## Process states
- running : Active process.
- sleeping : Idle process.
- Stopped : Process suspended by signal SIGSTOP (Ctrl+Z, Ctrl+C). It can be resumed by a SIGCONT signal.
- Zombie : The process has terminated, but its entry in the process table still exists because its parent process has not 
           yet read its exit status.
           
# 5 Commands used daily 
- ps or top : Provides process ID, memory usage, CPU time and command name which is crucial for monitoring system performance
              and troubleshooting.
- chmod : Changing permission of files.
- ssh : Provides secure shell connecting to remote server.
- systemctl : Managing system services (starting, stopping).
- df /du : df is used to monitor disk space usage and du is used to estimate size of a specific directory.
