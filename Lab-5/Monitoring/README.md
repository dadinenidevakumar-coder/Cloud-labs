This lab is about checking the performance of my Azure Virtual Machine using Azure Monitor, Metrics, and Logs (KQL).
I followed these steps:
1.Opened my VM and enabled Monitoring / Insights.
2.Checked CPU, Memory and Disk graphs from Metrics.
3.Opened Logs and ran some basic KQL queries.
4.Saved screenshots for each step.
KQL Queries I used
1.to check VM status
Heartbeat
| take 10
2.CPU details
Perf
| where ObjectName == "Processor"
| take 10
3.Memory details
Perf
| where ObjectName == "Memory"
| take 10
4.Disk
Perf
| where ObjectName contains  "Disk"
| take 10
also Screenshots included
Heartbeat query

CPU query

Memory query

Disk query. and Metrics graphs (CPU, Memory, Disk)
This lab helped me understand how to monitor a VM in Azure and how to run simple KQL queries to see logs.
