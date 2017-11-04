Linux Server Configuration

Linux distribution on a virtual machine, prepared to host web applications, install updates and securing it from a number of attack vectors.

i. The IP address and SSH port so your server can be accessed by the reviewer.
	a. IP address: 34.227.23.111
	b. SSH Port: 2200
ii. The complete URL to your hosted web application.
	a. http://ec2-34-227-23-111.compute-1.amazonaws.com/
iii. A summary of software you installed and configuration changes made.
Installed Packages

Package Name	
finger
apache2	
libapache2-mod-wsgi
ntp
postgresql
git
python-setuptools
sqlalchemy
flask
python-psycopg2
oauth2
google-api-python-client
requests

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