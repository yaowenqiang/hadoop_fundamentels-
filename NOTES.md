Hadoop Libraries

+ Mahoud - Machine learning algorithms
+ Spark - Resilient distributed data sets
+ Storm - Complex event processing


MapReduce Coding Patterns

+ Standard - usually written in java
+ Hadoop Streaming - Java base  Other language for mapper/reducer logic
+ Hadoop Pipes - uses C++
    


Hadoop shell Commands

> hadoop fs -cat file://file2
> hadoop fs -mkdir /user/hadoop/dir1 /usr/haddop/dir2
> hadooop fs -copyFromLocal <fromDir> <toDir>
- hadoop fs -put <localfile> hdfs://nn.example.com/hadoop/hadoopfile
> sudo hadoop jar <jarFileName> <method> <fromdir> <toDir>
> hadoop fs -ls /usr/hadoop/dir1
> hadoop fs -cat hdfs://nn1.example/file1
> hadoop fs -get /usr/hadoop/file <LocalFile>


MapReduce Libraries

+ import org.apache.hadoop.fs.Path;
+ import org.apache.hadoop.conf.*;
+ import org.apache.hadoop.io.*;
+ import org.apache.hadoop.mapred.*;;
+ import org.apache.hadoop.util.*;
1


Better MapReduce Optimizations

Optimize before the job runs.

+ File sizes
+ Compression
+ Encryption

Optimize onload of the data.

Optimize the map phase of the job.
Optimize the shuffle phase of the job.
Optimize the reduce phase of the job.
Optimize after the job completes.


Physical MapReduce Optimizations

+ Tip: Verify your cluster configuration parameters!
+ Do you have unused resources?
+ Do you have overstressed resources?
+ Are you using any type of cluster monitoring tools?

The Simplest Optimization is to add more nodes.


