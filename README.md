isOnline
========

Script for scheduled check for websites online status. Suited for crontab.

## Config
Create ```websites.txt``` file and fill it with each website in a new line (as in ```websites.txt.example```). leave an empty line in the end.

    Note that the script will approve http response 200 only. url with 301 (redirect) will fail.

## Add to crontab
Add the following lines to crontab config ($ crontab -e) 

```
THIS_IS_CRON=1
*/30 * * * * /path/to/isOnline/checker.sh
```

in this example crontab will run ```checker.sh``` every 30min.

by [ET][ET].

[ET]: http://etcs.me
