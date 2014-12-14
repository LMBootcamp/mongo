+------------------------------------------------------------------------------+
| Requirements                                                                 |
+------------------------------------------------------------------------------+
JDK 1.6 or later - Just a JRE is not sufficient, a full JDK is required
Maven 3.0.3 or later
mongo 2.2 or later

+------------------------------------------------------------------------------+
| Install Mongo and load test data                                                                |
+------------------------------------------------------------------------------+
See http://docs.mongodb.org/manual/installation/ form mongo installation instructions.

Navigate to the <mongo root>/bin directory and run the following command:

mongoimport -d blog -c posts <git repo path>/sampleData/posts.json

+------------------------------------------------------------------------------+
| Execute Maven and Launch the Web Container                                    |
+------------------------------------------------------------------------------+
For Linux/MAC users, execute the <git repo path>/javaCrudExample/run.sh

For windows users, run the following mvn command in the <git repo path>/javaCrudExample directory :

mvn compile exec:java -Dexec.mainClass=course.BlogController






