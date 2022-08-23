### Spark Shell 실행

```
$ cd $SPARK_HOME
$ ./bin/spark-shell
```

### org.apache.spark.SparkContext

```
scala> sc
```

### org.apache.spark.sql.SparkSession

```
scala> spark
```

### String = local\[\*\]

-   master node 정보 확인

```
scala> sc.master
```

### Option\[String\] = Some([http://172.16.100.49:4040](http://172.16.100.49:4040))

-   spark UI 정보

```
scala> sc.uiWebUrl
```

### SparkShell clear

```
scala> (Ctrl + L) 
```

### SparkShell exit

```
scala> :quit
```

### 프로세스 확인 (SparkSubmit)

-   Spark SHELL 밖에서

```
$ jsp
406
96633 Jps
95021 SparkSubmit
```

### Driver 웹UI 확인

```
http://spark-master-01:4040
```