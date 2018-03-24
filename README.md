# hdfs
Based on  sequenceiq/hadoop-docker:latest docker

 $HADOOP_PREFIX/bin/hadoop version

$HADOOP_PREFIX/bin/hdfs dfs -ls

$HADOOP_PREFIX/bin/hadoop fs -ls

Create local directory: 
mkdir usr/sumit 

Copy file from windows to container: 
docker cp names.csv f9d8c:/usr/sumit

Create directory in HDFS: 
$HADOOP_PREFIX/bin/hdfs dfs -mkdir sumith

Copy file from local to hdfs: 
$HADOOP_PREFIX/bin/hdfs dfs -put /usr/sumit/names.csv sumitH/names.csv

View files in hdfs:
$HADOOP_PREFIX/bin/hdfs  dfs -ls sumitH

View file contents in hdfs:
$HADOOP_PREFIX/bin/hdfs  dfs -cat sumitH/names.csv

remove the file from local, it will remain in hdfs

To display a table named 'newname' imported from sql server using sqoop 
$HADOOP_PREFIX/bin/hdfs dfs -cat newname/part-m-*
