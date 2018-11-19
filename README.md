##MongoDB Cookbook
 
###Starting a single node instance using command-line options
#####In this recipe, we will see how to start a standalone single node server with some command-line options. We will see an example where we want to do the following:

<ul>Start the server listening to port 27000</ul>
<ul>Logs should be written to /logs/mongo.log</ul>
<ul>The database directory is /data/mongo/db</ul>

The <b>/data/mongo/db </b>directory for the database and <b>/logs/ </b>for the logs should be created and present on your filesystem with appropriate permissions to write to it.
Execute the following command:

mongod --port 27000 --dbpath /data/mongo/db –logpath /logs/mongo.log --smallfiles