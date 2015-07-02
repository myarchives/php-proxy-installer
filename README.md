
# Install PHP-Proxy on your Server

The idea here is to simplify the installation process to the point where one-line is all that's needed to install and configure this app. Paste this command onto your terminal, and make sure you're doing this on a fresh server because this may remove some of your files.

```shell
bash <(wget -O - https://github.com/Athlon1600/php-proxy-installer/blob/master/install.sh)
```


### What does it do?

* apt-get update && apt-get upgrade
* Install Apache + PHP + cURL
* Enable mod_status, and automatically adjust Apache configuration based on the amount of RAM that server has.
* Install Composer
* Via Composer, Install [php-proxy-app](https://github.com/Athlon1600/php-proxy-app)
* Cron job to restart Apache every 12 hours
* Cron job to "composer update" the app every 24 hours.

### Soon to be added

* Automatically shut down the server once the bandwidth used exceeds XX terabytes/month.


Feel free to fork the project and add your own commands to fully personalize this for your own individual use.