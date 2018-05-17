# Create a data pipeline based on messaging using Spark and Hive

In this project, we will simulate a simple real-world batch data pipeline based on messaging using Spark and Hive.

**What are the prerequisites for this project?**

- Cloudera Quickstart VM
- Have a fair understand of Spark, Hive and how to use them

## What will you learn

- Designing a data pipeline based on messaging


- Load data from a remote URL


- Spark transformation


- Launching a Spark application from your application


- Explore hive as a backend for structured data access


- Discuss pipeline automation with Oozie or Airflow as another option

## Project Description

A data pipeline is a set of actions that are performed from the time data is available for ingestion till value is derived from that data. Such kind of actions is Extraction (getting value field from the dataset), Transformation and Loading (putting the data of value in a form that is useful for upstream use).

In this project, we will simulate a simple batch data pipeline. Our dataset of interest we will get from https://www.githubarchive.org/ that records over 20 kinds of events.

The objective of this spark project will be to create a small but real-world pipeline that downloads this dataset as they become available, initiated the various form of transformation and load them into forms of storage that will need further use.

The hackerday involves some form of software development, however, we will explore Spark and Hive while discussing some design decisions along the way.



GitHub Link:

https://github.com/okmich/githubarchive-analytics/tree/master/sample-data-pipeline

https://github.com/okmich/sample-data-pipeline