# limesurvey
docker-compose limesurvey container connecting to existing database. https://www.limesurvey.org/
This is an easy example of connecting to a local database with the use of dockers host.docker.internal passing the host ip.

# Docker image
This example uses one of the pre bult images in docker hub
For further details on the settings see: https://hub.docker.com/r/acspri/limesurvey

# Pre-Requirements
This example requires that you allready have a database running.
In my example i have an local mariadb running on port 3306. 
 - Create a new database called "limesurvey" in your existing db
 - create a new user names "limesurvey" with password "limesurvey" ( this you can change in production ) with all access to the limesurvey database.
 - All tables will be automatically created on docker startup.

# Run
`docker-compose up -d`
