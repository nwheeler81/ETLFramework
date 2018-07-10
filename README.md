# ETLFramework
OpenSource ETL project

## Start
### S3 to C*
dse -u cassandra -p cassandra spark-submit --jars ojdbc6.jar --class org.etl.ETL AMETLFramework-1.0-SNAPSHOT.jar -jobName ThirdJob -contactPoints 127.0.0.1 -login cassandra -passwd cassandra

### Oracle to C*
dse -u cassandra -p cassandra spark-submit --jars ojdbc6.jar --class org.etl.ETL AMETLFramework-1.0-SNAPSHOT.jar -jobName SecondJob -contactPoints 127.0.0.1 -login cassandra -passwd cassandra

### DSEFS to C*
dse -u cassandra -p cassandra spark-submit --jars ojdbc6.jar --class org.etl.ETL AMETLFramework-1.0-SNAPSHOT.jar -jobName FirstJob -contactPoints 127.0.0.1 -login cassandra -passwd cassandra
