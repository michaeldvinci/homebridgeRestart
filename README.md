# homebridgeRestart
Just for you, Derek -- make the files yourself, lol


Set up a cronjob to run every 2 hrs, or every [x] number of hours yo uwant, so it's at least 
automated?? I don't know how you want it timed

# Every two hours:
```bash
0 */2 * * *  /home/username/hbReboot.sh
```

# Every [x] number of hours:
```bash
0 */x * * *  /home/username/hbReboot.sh
```

# hbReboot.sh
```bash
sudo /etc/init.d/homebridge stop
sleep 5
sudo /etc/init.d/homebridge start
```
