# aws-elastic-beanstalk-demo
## How to Loging and Debuging Elastic BeanStalk
- Login using command eb ssh
- And you must create the file name must be same as the key name keypairt exist or attached the elasticbeanstlak, otherwise will not connect
- Switch to /var/log/eb-engin.log
- One of the biggest thing i had noticed you should zip the entire folder content not the folder from outside. Otherwise you’ll get     issue of composer.json missing or required.
- First is EB is deploy under path /var/app/stage then will install everything and moved  to /var/app/current.
The user in Elastic BeanStalk  webapp not www-data is chown -R webapp:webapp /var/app/staging

