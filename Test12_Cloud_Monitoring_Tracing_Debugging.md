# Cloud monitoring, tracing, and debugging 

## 1.- You are asked to create graphical dashboards for the operations team based on the logs recorded by your applications in Cloud Logging. Which Cloud Operations service would you use to perform this task? 

- a) Cloud Trace 
- b) **Cloud Monitoring**
- c) Cloud Debugger 
- d) Cloud Profiler 

RESUME: https://cloud.google.com/logging/docs/logs-based-metrics/charts-and-alerts

    To provide Cloud Monitoring with data from your logs, Logging offers you the following:
    - Log-based metrics, which you can use as follows:
        * To create alerting policies that notify you of changes over time.
        * To create charts that display changes over time.
    - Log-based alerts, which notify you anytime a specific event appears in a log.

## 2.- One of your applications is having performance problems and your hypothesis is that some code block is causing the problem. Which Cloud Operations service would you use to identify the problem? 

- a) Cloud Trace 
- b) Cloud Monitoring 
- c) Cloud Debugger 
- d) Cloud Profiler 

## 3.- Your application integrates with multiple external services and one of these is creating a bottleneck, but you don't know which one specifically. Which Cloud Operations service would you use to identify the bottleneck? 

- a) Cloud Trace 
- b) Cloud Monitoring 
- c) Cloud Debugger 
- d) Cloud Profiler

## 4.- You are having a problem in production that you have not been able to replicate in your development environment. If you could check the value of a variable of a particular line of code in production, you could solve this problem. Which Cloud Operations service would you use to perform this task? 

- a) Cloud Trace 
- b) Cloud Monitoring 
- c) Cloud Debugger 
- d) Cloud Profiler 

## 5.- Your application has critical flows for the user, whereby any problem in the latency of this flow can cause a reduction in business revenue. Which strategy would you use to ensure quality of service? 
- a) Create a cronjob that asks for the latency of the service every 10 seconds. 
- b) Configure service-level objectives (SLOs) associated with flow latency with Cloud Monitoring. 
- c) Divert all the requirements of that flow to BigQuery and have a team of analysts review the latency of each request. 
- d) Trust that the service will always work under the standards that are needed since we are in the cloud.
