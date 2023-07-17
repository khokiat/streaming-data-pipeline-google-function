# streaming-data-pipeline-google-function
## Description
In this project, Cloud Functions will stream and insert data to BigQuery (with Cloud Pub/Sub trigger). the function will make a REST API call to get a data and insert to BigQuery.

## Prerequisition&tool
1. **Cloud scheduler**
![image](https://github.com/khokiat/streaming-data-pipeline-google-function/blob/main/Picture/cloud-scheduler-512-color.max-600x600.png)
Cloud Scheduler is a fully managed enterprise-grade cron job scheduler. It allows you to schedule virtually any job.
2. **PUB/SUB**
![image](https://github.com/khokiat/streaming-data-pipeline-google-function/blob/main/Picture/download.png?raw=true)
a fully-managed, scalable, global and secure messaging service that allows you to send and receive messages among applications and services. In this projec, Pub/sub will send message to cloud function to streaming data by receiveing message from **cloud scheduler**
3. **Cloud function**
![image](https://github.com/khokiat/streaming-data-pipeline-google-function/blob/main/Picture/function.png)
Google Cloud Functions is a serverless execution environment for building and connecting cloud services. With Cloud Functions you write simple, single-purpose functions that are attached to events emitted from your cloud infrastructure and services. In this project we wil deploy code in here.

4. **Big query**
![image](https://raw.githubusercontent.com/khokiat/streaming-data-pipeline-google-function/da660e8b07eab83e09eb943a206877c5e368c2e7/bigquery.svg)
BigQuery is a fully managed enterprise data warehouse that helps you manage and analyze your data with built-in features like machine learning. By this project we will stream data to store in Big query.

## work flow
url = "https://randomuser.me/api/"

