Sometimes my WireGuard connections for peers that are behind firewalls or routers get dropped and they become inaccesible from outside. This simple script can be setup as a systemd-timer to check the connection and attempt to restart it when the endpoint cannot be reached. You can find examples service & timer in the `examples` directory.

Installaction is nothing fancy; just run `chmod +x wg-watchdog && sudo cp wg-watchdog /usr/local/bin` 

If you want to run as a systemd timer, take a look at the examples and customize to fit your system
