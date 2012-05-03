Run etsy-statsd from the daemontools

Recommended method:

* Copy the `run' file in this project into directory /etc/daemontools/statsd
* edit the `run' file and update the following 
       - NODE_JS - location of your node binary 
       - STATSD_JS - location of the statsd.js file
       - STATSD_CONFIG - location of your statsd config
       - USER - the user as which statsd will run
* create a softlink from /etc/service to /etc/daemontools/statsd
       - ln -sf /etc/daemontools/statsd /etc/service/statsd
