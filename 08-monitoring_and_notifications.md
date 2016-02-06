# Monitoring & Notifications

Log messages allow CHSDM staff to know when something has gone wrong. In the figures above, CHSDM staff can easily tell when things are working properly. Just as easily, CHSDM staff can start to notice when things are not working the way they should.

CHSDM staff use numerous services and tools to find out about problems quickly, and respond to them (and hopefully fix the problem) as soon as possible. Whenever something fails, it usually means visitors are stuck waiting, becoming frustrated and in general, not having a great experience. These are some of the tools that help CHSDM staff alleviate those frustrations.

* 
[Supervisord](http://supervisord.org/) - Monitors many of CHSDM services. If something has stopped, it tries to start it back up again.

* 
Watchdog - If the service can’t be restarted by Suporvisord, watchdog sends messages. These messages take the form of logs, but also alerts that wind up in CHSDM Slack channels.

* 
[New Relic](http://newrelic.com/) - This service monitors the health of CHSDM applications and servers. CHSDM staff can log into a dashboard and inspect all the data having to do with nearly all components of CHSDM systems. If a server is straining to keep up with its load, NewRelic sends an alert to Slack so CHSDM staff are alerted to the problem.

* 
[Pingdom](https://www.pingdom.com/) - This service continually checks if a website is working or not. If it’s not, it send CHSDM staff a text message and posts a message to Slack.

* 
[Slack](http://slack.com) - Slack is a tool CHSDM staff are using for internal communications. Additionally, Slack has become a hub for CHSDM staff alerting by many of the systems listed above.


