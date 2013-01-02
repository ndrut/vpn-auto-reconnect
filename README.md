# vpn-auto-reconnect
### A simple bash script for keeping an interface up, such as a vpn.

At the time of this writing, there's no known reconnection daemon or option for Fedora or the NetworkManager service that I can find. You can specify to "auto connect" however, that's not the same as reconnecting.


You can take this simple script and add a cron like:


```bash
*/5 * * * * /usr/bin/vpn-auto-reconnect >> /var/log/messages 2>&1
```


---

Feel free to fork/merge request if for some reason you want to make this better. ;)
