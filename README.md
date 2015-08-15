# P5: Linux Server Configuration

Project 5 for Udacity Full Stack Web Developer Nanodegree. 

This project includes baseline installation of a Linux distribution on a virtual machine and prepare it to host web applications, to include installing updates, securing it from a number of attack vectors and installing/configuring web and database servers.

## VM details
* IP address: 54.149.140.195
* SSH port: 2200
* URL: http://54.149.140.195

## Software installed
* apache and mod\_wsgi
* postgresql
* python-psycopg2
* pyton-pip
* flask
* oauth2client
* requests
* httplib2
* bootstrap
* ufw
* cron-apt

## Configuration changes to Catalog application
1. Add catalog.wsgi
2. Add new folder that contains catalog.wsgi and catalog source code. 
3. Change application.py to \_\_init\_\_.py
4. Add IP to google application ID source web site
5. Change web site in Facebook app console
6. Add variable APP\_ROOT to contain absolute path to client\_secrets.json and fb\_client\_secrets.json so that flow\_from\_client\_secrets function can find the two files.
7. Database locations have been pointed to postgresql to serve data.

## Configuration changes to server
1. Remote login of the root user is disabled
2. Key-based SSH authentication is enforced. Password login is disabled.
3. SSH port is changed from 22 to 2200
4. Applications have been updated to most recent updates.
5. cron-apt is installed to install updates at 4am everyday.
6. Apache has been configured with mod\_wsgi to serve flask applications. 

## Third-party resources
* https://help.ubuntu.com/community/SSH/OpenSSH/Keys
* https://help.ubuntu.com/community/AutoWeeklyUpdateHowTo


