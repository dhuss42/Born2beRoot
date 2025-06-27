# Born2beRoot

This project introduced me to virtualization and system administration. I successfully set up a secure Linux server on a virtual machine while following strict guidelines. I used VirtualBox and chose Debian Linux as my operating system.

## System Setup & Security

I configured my system without a graphical interface, ensuring a minimal and secure environment. My setup included:

- Partitioning: I created encrypted LVM partitions for better security.
- SSH Configuration: I set up SSH on port 4242, with root login disabled.
- Firewall Setup: I configured UFW to keep only port 4242 open.
- User Management: I created a non-root user with a strict password policy.
- Sudo Restrictions: I implemented limited authentication attempts, custom error messages, and logging of all sudo actions.

## Automated System Monitoring

I developed a Bash script that displayed key system stats every 10 minutes, including CPU usage, memory, disk space, network info, and active users. I automated its execution using cron jobs.

## Bonus

After completing the mandatory tasks perfectly, I went further by:

Hosting a WordPress site with lighttpd and MariaDB.
Installing Fail2ban
