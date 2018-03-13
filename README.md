# bhoptimer webstats panel

A partial rework and improvement of [Shavit's bhoptimer webserver module](https://github.com/shavitush/bhoptimer).

## Requirements

* bhoptimer using MySQL as the database host
* A webserver with PHP (tested on lighttpd 1.4.35 running php-cgi 5.6.33 on Debian 8)

### New Features

* Search all times by player name.
* Sort times by main or bonus track per map.

### Improvements

* Reworking of SQL to support database changes in modern (as of March 2018) bhoptimer.
* Future support for multiple bonus stages.

### Installation

1. Edit config.php to suit your needs. If your MySQL server is not hosted on the same server as the webserver, you'll have to configure it and ensure the user you use has SELECT privileges on the shavit database.
2. Upload all .php files as well as the /assets folder.
3. Browse to /index.php, if maps appear in the nav bar dropdown everything should be in working order.