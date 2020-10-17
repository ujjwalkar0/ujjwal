---
title: How to setup postgresql and pgadmin in your Ubuntu Laptop ?
date: 2020-10-17T16:22:52.092Z
draft: false
featured: false
image:
  filename: featured
  focal_point: Smart
  preview_only: false
---
## Install Postgresql

```
# Create the file repository configuration:
sudo sh -c 'echo "deb http://apt.postgresql.org/pub/repos/apt $(lsb_release -cs)-pgdg main" > /etc/apt/sources.list.d/pgdg.list'

# Import the repository signing key:
wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | sudo apt-key add -

# Update the package lists:
sudo apt-get update

# Install the latest version of PostgreSQL.
# If you want a specific version, use 'postgresql-12' or similar instead of 'postgresql':
sudo apt-get -y install postgresql
```



## Make Sure You have installed following packages

python-dev, build-essential, libssl-dev, libffi-dev, libxml2-dev, libxslt1-dev, zlib1g-dev, python3.x-pip, python3.x-dev  (x is your version)

```
sudo apt-get install python-dev
sudo apt-get install build-essential
sudo apt-get install libssl-dev
sudo apt-get install libffi-dev
sudo apt-get install libxml2-dev
sudo apt-get install libxslt1-dev
sudo apt-get install zlib1g-dev
sudo apt-get install python3.x-pip
sudo apt-get install python3.x-dev
```



## Install PgAdmin4 

```
$ sudo mkdir /var/lib/pgadmin
$ sudo mkdir /var/log/pgadmin
$ sudo chown $USER /var/lib/pgadmin
$ sudo chown $USER /var/log/pgadmin
$ python3 -m venv pgadmin4
$ source pgadmin4/bin/activate
(pgadmin4) $ pip install pgadmin4
...
(pgadmin4) $ pgadmin4
NOTE: Configuring authentication for SERVER mode.

Enter the email address and password to use for the initial pgAdmin user account:

Email address: user@domain.com
Password: 
Retype password:
Starting pgAdmin 4. Please navigate to http://127.0.0.1:5050 in your browser.
 * Serving Flask app "pgadmin" (lazy loading)
 * Environment: production
   WARNING: Do not use the development server in a production environment.
   Use a production WSGI server instead.
 * Debug mode: off
```