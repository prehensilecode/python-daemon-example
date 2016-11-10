# python-daemon-example
Simple example of using python-daemon with logging and PID lock file.

What is here:
* eg_daemon.py -- the Python-based daemon itself; should be installed in /var/lib/eg_daemon/
* eg_daemon.init -- SysV init script; should be installed in /etc/init.d

When eg_daemon.py is started, these two files will be created:
* /var/run/eg_daemon.pid -- this file will contain the PID of the daemonized process; 
                            it is automatically deleted when the daemon is stopped normally
* /var/log/eg_daemon.log -- log file

