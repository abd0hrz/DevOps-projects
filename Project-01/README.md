### In this project, I manually created VMs with Vagrantfile for a 3-Tier Application Stack setup "MySQL/MariaDB, Memcached, RabbitMQ, Tomcat and Nginx" using bash script to manually configure Linux servers.

I used Maven to build the artifact which was deployed to the Tomcat server.
---------------------------------------------------------------------
### Setup Flow:
#### ✅ Using vagrant, I created VMs via oracle VB
#### ✅ Logged into every machine and manually executed shell commands using Bash
#### ✅ I set up my services.
#### ✅ Once the stack was ready, I verified as the user from the browser.
#### ✅ I accessed the Nginx service which then forwarded the request to the tomcat server, which then forwarded that request to message broker RabbitMQ, then to Memcached, and lastly to the MySQL server. The query executed on the tomcat server was then cached to the Memcache server

## Read Detailed Documentation from link below...
#### https://medium.com/@osomudeyazudonu/project-1-vprofile-project-multi-tier-web-application-stack-setup-locally-59ef7917fc42




# Prerequisites
#
- JDK 1.8 or later
- Maven 3 or later
- MySQL 5.6 or later

# Technologies 
- Spring MVC
- Spring Security
- Spring Data JPA
- Maven
- JSP
- MySQL
# Database
Here,we used Mysql DB 
MSQL DB Installation Steps for Linux ubuntu 14.04:
- $ sudo apt-get update
- $ sudo apt-get install mysql-server

Then look for the file :
- /src/main/resources/accountsdb
- accountsdb.sql file is a mysql dump file.we have to import this dump to mysql db server
- > mysql -u <user_name> -p accounts < accountsdb.sql


