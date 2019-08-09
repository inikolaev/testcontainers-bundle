# TestContainers Bundle

This is a fat jar containing all dependencies required to start PostgreSQL container. 
I created it so that I could use it as a JDBC driver in JetBrains DataGrip which now allows me to start new database from a Docker image and connect to it.

## Configuration

1. Download `testcontainers-bundle` jar from releases and add it as new JDBC driver in DataGrip 
2. Create new database connection and specify JDBC URL similar to this: `jdbc:tc:postgresql://hostname/databasename`
3. Now you can use your database

## Issues

* Right now database container is destroyed as soon as database connection is closed
