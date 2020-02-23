Sometimes my WireGuard connections for peers that are behind firewalls or routers get dropped and they become inaccesible from outside. This simple script can be setup as a systemd-timer to check the connection and then attempt to restart it the endpoint can't be reached. You can find examples service & timer in the `examples` directory.

Installaction is nothing fancy; just run `chmod +x wg-watchdog && cp wg-watchdog /usr/local/bin` 
