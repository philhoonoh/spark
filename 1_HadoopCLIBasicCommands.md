# Hadoop version 확인

```
$ hadoop version
```

# Hadoop dfs 실행

```
$ cd $HADOOP_HOME
$ sbin/start-dfs.sh
$ sbin/stop-dfs.sh
```

# Hadoop yarn 실행

```
$ cd $HADOOP_HOME
$ sbin/start-yarn.sh
$ sbin/stop-yarn.sh
```

# hadoop hdfs CLI 사용

```
- (아래 2개 동일)
- prefix 같이 사용 
$ hdfs dfs
$ hadoop fs 
```

# hadoop hdfs CLI + Linux 명령어 형식

```
$ hadoop fs -mkdir /user/philhoonoh/input
$ hadoop fs -ls /user/philhoonoh
```

# put : Local -> HDFS

```
$ hadoop fs -help put
$ hadoop fs -put LICENSE.txt /user/philhoonoh/input
$ hadoop fs -ls /user/philhoonoh/input
```

# copyToLocal : HDFS -> Local

```
$ hadoop fs -help get
$ hadoop fs -help copyToLocal
$ hadoop fs -copyToLocal /user/philhoonoh/input/LICENSE.txt ./
```

# HDFS 상의 파일 cat

```
$ hadoop fs -cat /user/philhoonoh/input/LICENSE.txt
```

# HDFS 상의 파일 mv, cp, rm

```
$ hadoop fs -mv /user/philhoonoh/input/LICENSE.txt /user/philhoonoh
$ hadoop fs -cp /user/philhoonoh/LICENSE.txt /user/philhoonoh/input/
$ hadoop fs -rm /user/philhoonoh/LICENSE.txt
```

# HDFS 상의 파일 head, tail

```
$ hadoop fs -tail /user/philhoonoh/input/LICENSE.txt
$ hadoop fs -head /user/philhoonoh/input/LICENSE.txt
```

# HDFS 상의 명령어 help

```
$ hadoop fs -help [명령어]
$ hadoop fs -help cp
```