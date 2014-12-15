##Requirements

JDK 1.6 or later - Just a JRE is not sufficient, a full JDK is required

maven 3.0.3 or later

mongo 2.2 or later

##Install Mongo and load test data

See http://docs.mongodb.org/manual/installation/ form mongo installation instructions.

Launch mongod if it is not running already (<<mongo root>>/bin/mongod)

Navigate to the <<mongo root>>/bin directory and run the following command:

mongoimport -d blog -c posts <<git repo path>>/sampleData/posts.json

##Execute Maven and Launch the Web Container

For Linux/MAC users, execute the <git repo path>/javaCrudExample/run.sh

For windows users, run the following mvn command in the <git repo path>/javaCrudExample directory :

mvn compile exec:java -Dexec.mainClass=course.BlogController

If the above script or maven command executes successfully, you should be able to login or create a blog account via the link below:

See http://localhost:8082/login





