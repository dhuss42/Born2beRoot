# Born2beRoot

## Contents

1. [Project Overview](#1-Project-overview)
2. [Mandatory Part](#2-Mandatory-Part)
3. [Bonus](#3-Bonus)

## 1. Project Overview

This project introduced me to virtualization and system administration. I successfully set up a secure Linux server on a virtual machine while following strict guidelines. I used VirtualBox and chose Debian Linux as my operating system. Due to it's large size it is not suitable for uploading to Github. Therefore this repository only covers briefly what the project was about.

## 2. Mandatory Part

I configured my system without a graphical interface, ensuring a minimal and secure environment. My setup included:

- Partitioning: I created encrypted LVM partitions for better security.
- SSH Configuration: I set up SSH on port 4242, with root login disabled.
- Firewall Setup: I configured UFW to keep only port 4242 open.
- User Management: I created a non-root user with a strict password policy.
- Sudo Restrictions: I implemented limited authentication attempts, custom error messages, and logging of all sudo actions.

I developed a Bash script that displayed key system stats every 10 minutes, including CPU usage, memory, disk space, network info, and active users. I automated its execution using cron jobs.

## Bonus

After completing the mandatory tasks perfectly, I went further by impleting the following services.

WordPress
WordPress is an open-source content management system that allows you to build and manage websites or blogs easily through a user-friendly web interface. In the project, I deployed WordPress to create a simple dynamic website hosted on my server.

lighttpd
lighttpd is a lightweight, high-performance web server optimized for speed-critical environments. It uses minimal resources compared to heavier web servers like Apache, making it a good choice for serving websites on low-powered systems or virtual machines. In this project, I configured lighttpd to serve my WordPress site efficiently.

MariaDB
MariaDB is an open-source relational database management system. It’s widely used with web applications to store and manage data such as website content or user information. In this project, I used MariaDB to store the database for my WordPress installation, ensuring reliable and fast data access.

Fail2Ban
Fail2Ban is a security tool that scans log files for suspicious activity, like repeated failed login attempts, and automatically updates firewall rules to ban offending IP addresses. This helps protect services such as SSH or web servers from brute-force attacks. In my project, I installed and configured Fail2Ban to secure my server from unauthorized access attempts.
