# bhoptimer webstats panel

A partial rework and improvement of [Shavit's bhoptimer webserver module](https://github.com/shavitush/bhoptimer).

## Requirements

* bhoptimer using MySQL as the database host. SQLite is unsupported.
  * To display Top Players (as is default), shavit-wr and 
shavit-rankings are also required.
  * Highly recommended to have your database [configured per this article](https://github.com/shavitush/bhoptimer/wiki/4.2.-Extra:-Updating-(Database))
* A webserver with PHP (tested on lighttpd 1.4.35 running php-cgi 5.6.33 on Debian 8)
  * If you want to use vanity URL searching, php-curl must be installed as well.

### Features

* View top times for each map, organized by style.
* Each user's time displayed along with their SteamID and a link to 
their Steam Community page.

### New Features

* Search all times by player name, SteamID3/32/64 or Steam Community URL.
* Sort times by main or bonus track per map.
* View Top Players on the server, sorted by points.
* Quickly jump between rankings on a given map, style and player.

### Improvements

* Reworking of SQL to conform with database changes in modern (as of March 2018) bhoptimer.
* Inclusion of statistics like jumps/strafes/sync.
* Future support for multiple bonus stages.

### Installation

1. Edit config.php to suit your needs. If your MySQL server is not 
hosted on the same server as the webserver, you'll have to configure it 
and ensure the user you use has SELECT privileges on the shavit 
database. If your server uses custom/non-default styles, change the 
$styles array accordingly. 
2. Upload all .php files as well as the /assets folder.
3. Browse to /index.php, if maps appear in the nav-bar dropdown everything should be in working order.

### Live Demo

https://bhop.crap.site
