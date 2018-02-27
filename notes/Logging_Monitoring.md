Logging, Monitoring and User notifications
==========================================

There are many ways to get notifications
-----------------------------------------
- LSST Slack bots are almost real personalities in LSST 
- Challenge: Microservice to match github id and slack user (LSST)
- SciServer also uses Slack for admin notifications
- DES uses email post and Jira tickets
- Set levels for alerts defined by system usage

How to unified logging information
----------------------------------
- SciServer uses RabbitMQ and MYSQL to store structured data
- DES uses Redis and fluend and influxDB
- [Fluentd](https://www.fluentd.org/) is a growing solutions (being adopted by DES)
  logging infrastructure (at NCSA)
- Need a efficient way to store but also retrieve log information accumulated over time
- Separate logging information from admins and users
- ElasticSearch
- Need to log the logging system, maybe a single failure point
- Common data format for logging

Monitoring
----------
- LSST Squash to monitor building stack, very useful for debugging when there are many packages being build, can be tracked to the commit level
- There is a general need to monitor system and user activity
- Demographics information is great but a blocker in registration, but can provide a great deal of information
- Collect information of the system to be able to predict the system before it fails
- LSST plans to allow users (DM users?) to collect their own metrics, using JSON
- Kubernetes monitoring, pods, deployments,services, access
- User activity is important to schedule and manage resources, (work during night/day, work/home, )
