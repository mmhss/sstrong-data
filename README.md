### Set up a database with Liqubase - database schema change management 

Update the following connection properties in pom.xml to connection to the database. Create an empty database of your choice at first.
```
<url>jdbc:mysql://server-name:3306/database-name</url>
<username>username</username>
<password>password</password>
```

The following command will build the database.
```
mvn install
mvn liquibase:update
```

### Sample Data
The passive sensing data - GPS, Activty, Proximity beacon and Audio prediction flat files are available in the sample-data folder [sample-data](sample-data/). 
