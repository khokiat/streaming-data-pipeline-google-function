# streaming-data-pipeline-google-function
## Description
In this project, Cloud Functions will stream and insert data to BigQuery (with Cloud Pub/Sub trigger). the function will make a REST API call to get a data and insert to BigQuery.
![image](https://github.com/khokiat/streaming-data-pipeline-google-function/blob/main/Picture/Pipeline%20architecture.jpg?raw=true)

## Prerequisition&tool
1. **Cloud scheduler**
Cloud Scheduler is a fully managed enterprise-grade cron job scheduler. It allows you to schedule virtually any job.
2. **PUB/SUB**
a fully-managed, scalable, global and secure messaging service that allows you to send and receive messages among applications and services. In this projec, Pub/sub will send message to cloud function to streaming data by receiveing message from **cloud scheduler**
3. **Cloud function**
Google Cloud Functions is a serverless execution environment for building and connecting cloud services. With Cloud Functions you write simple, single-purpose functions that are attached to events emitted from your cloud infrastructure and services. In this project we wil deploy code in here.

4. **Big query**
BigQuery is a fully managed enterprise data warehouse that helps you manage and analyze your data with built-in features like machine learning. By this project we will stream data to store in Big query.

5. **Resource API**
url = "https://randomuser.me/api/"

## Step to run
1. Create Dataset, table and specified schema in Big Query
2. Create cloud function instance by specify dataset and table name including url that we need to make API call in project.
3. Create PUB/SUB to trigger service.
4. Deploy streaming code into Cloud function.
5. Compose cloud scheduler to control schudule and trigger pipeline by setting  pub/sub trigger matched to trigger that we've set in cloud function. 

![image](https://github.com/khokiat/streaming-data-pipeline-google-function/blob/main/Picture/Image%2017-7-2566%20BE%20at%2015.25.jpg?raw=true)
