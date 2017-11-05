Linux Server Configuration

Linux distribution on a virtual machine, prepared to host web applications, install updates and securing it from a number of attack vectors.

i. The IP address and SSH port so your server can be accessed by the reviewer.
	
	a. IP address: 13.59.95.154

	b. SSH Port: 2200

ii. The complete URL to your hosted web application.
	
	a. http://ec2-13-59-95-154.us-east-2.compute.amazonaws.com

iii. A summary of software you installed and configuration changes made.

Installed Packages

Package Name	
1. finger
2. apache2
3. libapache2-mod-wsgi
4. ntp
5. postgresql
6. git
7. python-setuptools
8. sqlalchemy
9. flask
10. python-psycopg2
11. oauth2
12. google-api-python-client
13. requests

Configuration Summary

1. Setup Virtual Machine and SSH into the server.
2. A new system user grader was created with permission to sudo.
3. All cuurently installed packages were updated and upgraded.
4. CRON tasks added to update and upgrade installed packages.
5. Changed SSH Port from 22 to 2200 and configure SSH access.
6. Configured UFWto only allow incoming connections for SSH(Port:2200), HTTP(Port:80) and NTP(Port:123).
7. Configured local Time Zone to UTC.
8. Installed and configure Apache to serve a Python mod_wsgi application.
9. Installed Git and Setup Environment for delopying Flask Application.
10. Install and configure PostgreSQL with default settings to not allow remote connection.
11. Created a new user catalog, added user to PostgreSQL databse with limited permissions to catalog application database.
12. Get OAUTH-LOGINS (Google+) working.
