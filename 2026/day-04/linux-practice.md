# Real time output of commands I practiced

## Process commands
* `ps -aux | head -n 10` - List running processes(top 10 lines).
![snapshot](images/psaux.png)
* `pgrep -x sshd` - Get the process id by process name.
![snapshot](images/pgrep.png)

## Service commands
* `systemctl status | head -n 20` - Prints first 20 lines of system service status summary.
![snapshot](images/systemctl.png)
* `systemctl list-units --type=service --state=running | head` - Prints first 10 lines of running services status.
![snapshot](images/systemctl_listunits.png)

## Log commands
* `journalctl -u ssh` - Displays logs for the SSH service.
![snapshot](images/journalctl.png)
* `tail -n 40 /var/log/auth.log` - Last 40 lines of the authentication log(ssh, sudo).
![snapshot](images/tail.png)

## Service for inspection (SSH)
`systemctl status ssh`
![snapshot](images/ssh.png)

It is running now lets stop it. And try to connect to localhost.
![snapshot](images/stopservice.png)

Giving error 
![snapshot](images/error.png)

Let's view logs and check
![snapshot](images/logs.png)

Log shows the service is stopped let's start the ssh service and check again
![snapshot](images/started.png)

Service started and localhost connection made
