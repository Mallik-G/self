# Spark SQL on Spark 2

In this hackerday, we will explore the features of Spark SQL in practice.



## What will you learn

- What is Spark SQL


- Why you should think Spark SQL before Spark Core


- When you are going to have to use Spark Core


- Spark SQL and multiple file types: Text File, JSON File, RDBMS Sources, NoSQL Sources


- Spark SQL for SQL-on-Hadoop server


- Introduction to Spark Structured Streaming

## Prerequisites

- It is expected that students have a fair knowledge of Big Data and hadoop particularly [HDFS](https://www.dezyre.com/hadoop-course/hdfs), [Spark](https://www.dezyre.com/apache-spark-scala-training-online/38) and [Hive](https://www.dezyre.com/hadoop-course/hive).


- Installation Cloudera QuickStart VM.


- Since we will be doing the development in the Quickstart VM, it is essential to have the Scala SDK installed there as well. Instruction on how to set up a Scala SDK and runtime can be found at [here](https://www.youtube.com/watch?v=SFJsuo2XISs&t=151s).


- In the class, we will do an installation of Spark 2 in the Cloudera Quickstart VM. By default, the VM comes pre-installed with Spark 1.6.x.

## Project Description

Spark 2 offers a huge but yet backward-compatible break from the Spark 1.x, not only in terms of high-level API but also in performance. And spark the module with the most significant new features is Spark SQL.

In this hackerday, we will explore a number of this features in practice.

We will discuss using various dataset, the new unified spark API as well as the optimization features that makes Spark SQL the first way to explore in processing structured data.

However, there are times when it is inevitable to resort to Spark Core - RDD in Spark 2. We will explore that as well alongside the newest and cool structured streaming API that enables fault-tolerant stream processing engine built on the Spark SQL engine.



Code: https://github.com/okmich/spark-exercises