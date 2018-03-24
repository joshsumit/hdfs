# hdfs
Based on  sequenceiq/hadoop-docker:latest docker

$HADOOP_PREFIX/bin/hdfs dfs -ls
$HADOOP_PREFIX/bin/hadoop fs -ls

create local directory: mkdir usr/sumit 
copy file from windows to container: docker cp names.csv f9d8c:/usr/sumit

create directory in HDFS: $HADOOP_PREFIX/bin/hdfs dfs -mkdir sumith
copy file from local to hdfs: $HADOOP_PREFIX/bin/hdfs dfs -put /usr/sumit/names.csv sumitH/names.csv
view files in hdfs $HADOOP_PREFIX/bin/hdfs  dfs -ls sumitH

view file in hdfs
$HADOOP_PREFIX/bin/hdfs  dfs -cat sumitH/names.csv



