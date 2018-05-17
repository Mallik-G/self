# **Hadoop Project based Training**

# Projects you will work on

In this program, you'll work on real world Big Data problems. You will learn how to choose the right Big Data technologies, load data, analyze data and perform configuration management.

#### **Introduction to Hadoop**

In the first class - we will learn about Big Data, Hadoop and MapReduce concepts. We will setup Cloudera Quickstart VM and go over Hadoop installations. The faculty will guide you on how to access all datasets and setup your github accounts.

https://github.com/okmich/hadoop-training-projects/blob/master/steps_to_setup_cloudera_quickstart_vm.txt

#### **Project 1 - Ingest Sakila film database using Sqoop**

In this project we will learn to install and play around with importing and exporting data with Sqoop. First we will import the MySQL World database tables into HDFS with default delimiters and using non-default file formats. Then we will practice by importing the Sakila film database tables into HDFS. Finally, we will export a parquet file on customer data from HDFS to MySQL.

https://github.com/okmich/hadoop-training-projects/tree/master/sqoop

#### **Project 2 - Ingest Twitter data using Flume**

In this project we will build a Flume agent to ingest data from Directory spool source to HDFS. We will be using interceptors and channel selectors. We will then use the famous Twitter example and build a Flume agent to stream data from Twitter to HDFS.

https://github.com/okmich/hadoop-training-projects/tree/master/flume

#### **Project 3 - Processing Movielens dataset using Pig**

In this project, we will learn about Apache Pig and how to use it to process the Movielens dataset. We will get familiar with the various Pig operators used for data processing. We will cover how to use UDFs and write your own custom UDFs. Finally we will take a look at diagnostics and performance tunning.

https://github.com/okmich/hadoop-training-projects/tree/master/pig

#### **Project 4 - Processing NYSE trading data using Hive**

In this project we will learn about Apache Hive - another popular processing framework. We will be using Hive to process the NYSE trading data on daily price. We will see the different file types and formats available and how to create and load data into Hive tables. Finally we will show how partitioning works in Hive.

https://github.com/okmich/hadoop-training-projects/tree/master/hive

https://github.com/rashmireddy/dezyre-nyse



#### **Project 5 - Querying Airline on-time performance dataset using Hive**

We will dive deeper into Hive in this project. We will be working with the airline on-time performance dataset. As part of processing this data - we will learn about Joins. We will also learn how to use built in UDFs and also create your custom UDFs/UDAFs.

https://github.com/okmich/hadoop-training-projects/tree/master/hive

#### **Project 6 - Workflow and Cordination for Movielens data using Oozie**

Here we will be introducing the workflow manager - Oozie. We will learn how to create and run an oozie 

work flow for movielens data processing pipeline. We will be using the Pig and Hive actions to setup this work flow. We will also be building Oozie coordinators using Time and data triggers.

https://github.com/okmich/hadoop-training-projects/tree/master/oozie

#### **Project 7 - Twitter Feed Analysis**

This is our final project and will be using multiple tools we have learnt through the course. We will be loading live twitter feeds related to jobs advertisements. We will setup batch processing of tweets on hdfs and then extract the data to MySQL database. We will also use Oozie as workflow manager.

https://github.com/okmich/hadoop-training-projects/tree/master/final_project

