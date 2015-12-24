# Overview
Vanilla is a powerful open source web-based forum.  this charm will deploy the forum software and conneect it to a running MySQL database. This charm will install the Vanilla files in /var/www/vanilla/
# Installation 
To deploy this charm you will need at a minimum: a cloud environment, working Juju installation and a successful bootstrap.  Once bootstrapped, deploy the MySql charm and then thisV anilla charm:
    juju deploy mysql
    juju deploy vanilla
Add a relation between the two of them:
    juju add-relation mysql vanilla
And finally expose the vanilla service:
    juju expose vanilla
