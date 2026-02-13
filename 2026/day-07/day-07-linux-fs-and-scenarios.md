Scenario 1: Service Not Starting
A web application service called 'myapp' failed to start after a server reboot.
What commands would you run to diagnose the issue?

Step 1: systemctl status nginx
Why: This command shows the status of the service if it is running or stopped.

Step 2: systemctl is-enabled nginx
Why: This command tells if the service will automatically boot on restarting the system or not.

Step 3: journalctl -u nginx -n 50
Why: This command shows last 50 logs of the specific service in human readable format.

Step 4: netstat -tulpn | grep :80
Why: This commands give information if the required port is in use or available. It  also tell which service is using the mentioned port.

Scenario 2: High CPU Usage
Your manager reports that the application server is slow.
You SSH into the server. What commands would you run to identify
which process is using high CPU?

Step 1: top
Why: This command display CUP and RAM usage.

Step 2: htop
Why: It is advanced version of top command.

Step 3: Step 1: ps aux --sort=-%cpu | head -10
Why: This command lists top 10 CPU comsuming procees.

Step 4: kill <PID>
Why: After getting process id using top user can kill or stop that PID.

Scenario 3: Finding Service Logs
A developer asks: "Where are the logs for the 'nginx’ service?"
The service is managed by systemd.
What commands would you use?


Step 1: systemctl status nginx
Why: This command shows if the service is running or not.

Step 2: journalctl -u ssh -n 50
Why: This command shows last 50 logs for this service. 

Step 3: journalctl -u nginx -f
Why: This command shows rea time logs.

Step 4: journalctl -u nginx -p 3 -f
Why: This command only shows logs with error message.

Step 1: Check current permissions
Command: ls -l /home/user/backup.sh
Look for: -rw-r--r-- (notice no 'x' = not executable)

Step 2: Add execute permission
Command: chmod +x /home/user/backup.sh

Step 3: Verify it worked
Command: ls -l /home/user/backup.sh

Step 4: Try running it
Command: ./backup.sh


