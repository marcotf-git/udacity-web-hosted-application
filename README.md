# Web Hosted Application

This project is an exercise as part of the **Full Stack Web Developer Nanodegree**, by **Udacity**. It is an exercise of hosting a web application! 😃 It takes a baseline installation of a Linux distribution and prepare it to host a web application by installing updates, securing it from a number of attack vectors and installing and configuring web and database servers.

The web application is a **Catalog App**. It provides a list of items within a variety of categories and integrate third-party user registration and authentication, besides the possibility of local authentication. Because the site does not have  a domain name, the functionality of third party authentication is not working at the moment, but it was tested and works in *localhost*.

The server can be accessed through `ssh` at `IP 18.221.18.203`  port `2200`.

The application can be accessed at `<http://18.221.18.203/>`.

This hosted web application is for learning purposes. 📚

# Summary of installed software and configuration

* The system software was updated.

* The `Firewall` was setup, making incoming permissions to allow only the services needed `www` (port 80) `ssh` (port 2200) `ntp` (port 123, `udp`) (🔴 take care or you will lose the connection!).

* The `ssh` listening port was changed to `2200`.

* It was generated a new key-pair and installed the public key in the server.

* After that (✋ take care or you will lose the connection!) the authentication method was configured to be key based only.

* Installed the **Apache** server `apache2`.

* Installed the **WSGI** module `libapache2-mod-wsgi` for handling the **Python 2.7** application.

* Installed **PostgreSQL** database (`postgresql`).

* Installed **Git** (`git`).

* Configured the **Apache** (`/etc/apache2/sites-enables/000-default.conf`) to handle the `wsgi` **Python** application.

* Configured the **Python** `load path` to the application.

* Created a  new database user named `catalog` with limited permissions to the application database.

* Adapted the software to handle `postgresql` database.

* Corrected application runtime error `IO error` by making absolute reference `url` when loading files.


# Credits

These are some useful links, in addition to **Udacity** itself, that were queried in this project:

https://www.digitalocean.com/community/tutorials/how-to-install-linux-apache-mysql-php-lamp-stack-on-ubuntu-14-04

https://www.digitalocean.com/community/tutorials/how-to-install-and-use-postgresql-on-ubuntu-14-04

https://www.digitalocean.com/community/tutorials/how-to-secure-postgresql-on-an-ubuntu-vps

https://www.digitalocean.com/community/tutorials/7-security-measures-to-protect-your-servers

http://httpd.apache.org/docs/current/configuring.html

*Important Python instructions:*

http://flask.pocoo.org/docs/0.12/deploying/mod_wsgi

http://docs.sqlalchemy.org/en/latest/core/engines.html#database-urls


Thank You!
