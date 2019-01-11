# c-rieger.de - install Nextcloud using a shell script
The initial script called install-nextcloud-ubuntu.sh or install-nextcloud-debian.sh (depending on your server os) will install your self hosted Nextcloud within few minutes, fully prepared for Ubuntu 18.04 or Debian 9.6 Stretch environments and will consist of:

    Fail2Ban (Nextcloud and SSH jails)
    MariaDB 10.3
    Nextcloud 15 latest
    NGINX 1.15.8
    OpenSSL 1.1.1 + TLS v. 1.3
    PHP 7.3
    Redis-Server
    self signed or Let’s Encrypt SSL using the second script
    UFW (22, 80, 443)

Requirements:

    Ubuntu 18.04 or Debian 9.6
    Please remove already installed packages of NGINX, PHP, MariaDB and Redis first or start with a new server os!

    apt purge <package> -y && apt autoremove -y

Beyond that you will find additional scripts at /usr/local/src/install-nextcloud/

    /maintainance/fail2ban.sh
    /maintainance/ubuntu/optimize-ubuntu.sh
    /maintainance/debian/optimize-debian.sh
    /maintainance/restart.sh
    /maintainance/ssl-renewal.sh
    /maintainance/ubuntu/upgrade-ubuntu.sh
    /maintainance/debian/upgrade-debian.sh
    /ssl/ssl-certificate-debian.sh
    /ssl/ssl-certificate-ubuntu.sh

to optimize and maintain your system easily. Ready to go? Let’s start:

Carsten Rieger IT-Services (c-rieger.de)
