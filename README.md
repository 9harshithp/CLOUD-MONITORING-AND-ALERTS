# CLOUD-MONITORING-AND-ALERTS
**COMPANY**: CODTECH IT SOLUTIONS

**NAME**: HARSHITH P

**INTERN ID**:CT08IJR

**DOMAIN**: Cloud Computing

**BATCH DURATION**: January 30th, 2025 to March 1st, 2025

**MENTOR NAME**: NEELA SANTHOSH

**ENTER DESCRIPTON OF TASK PERFORMED NOT LESS THAN 500 WORDS**:
For this task, I set up a comprehensive monitoring system for my cloud-based application using AWS CloudWatch. The primary goal was to ensure that I could keep an eye on my EC2 instance’s performance, especially in terms of resource usage, and be alerted when things started to go awry. Here’s a breakdown of what I did:

1. Creating the Log Group:
The first thing I did was create a CloudWatch Log Group. I named it MyAppLogs to make it easy to identify as the log group dedicated to my application’s logs. This log group will store all the logs related to my app, which can be critical for troubleshooting and performance analysis.

For log retention, I chose the Never expire option. This was intentional because I wanted to make sure no logs are deleted by accident over time. Keeping logs for a longer duration can be helpful in understanding long-term trends, solving issues that arise later, or just for historical reference. As for the log class, I went with the default Standard class. It offers the right balance of durability and availability, which is exactly what I need for my use case.

2. Configuring the Alarm:
Once the log group was in place, the next step was to configure an alarm to monitor the performance of my EC2 instance. I focused on monitoring CPU utilization because it’s one of the most common indicators of system load. I set the alarm to trigger when the CPU utilization exceeds 80% for more than 5 minutes. However, I decided to set a more conservative threshold of 5% CPU utilization. This threshold would allow me to monitor even smaller fluctuations and act on them promptly, reducing the risk of overlooking early performance issues. I thought this would be a good threshold to catch any performance issues while avoiding false alarms caused by temporary spikes.

For notifications, I configured Amazon SNS (Simple Notification Service). This way, whenever the alarm is triggered, I would receive an instant notification—whether via email, SMS, or another method. I wanted to make sure that if something went wrong, I would be able to react quickly.

3. Setting Up the Dashboard:
With the log group and alarm set up, I then created a CloudWatch Dashboard called MyAppDashboard. This dashboard will be my central place for viewing the real-time health of my application. I decided to use a line graph widget because it’s great for tracking how things are changing over time, especially metrics like CPU utilization.

The dashboard is helpful because it gives me a quick overview of the EC2 instance’s performance. With the line graph, I can easily see if there’s a trend toward higher CPU usage or if everything is running smoothly. This kind of visualization is crucial for identifying issues early on before they turn into bigger problems.

4. Bringing It All Together:
The final step was to integrate all the pieces—log group, alarm, and dashboard—into a cohesive monitoring system. The log group ensures all logs are captured and stored, the alarm provides an early warning system for high CPU utilization, and the dashboard gives me a visual tool to track performance.

Having this setup in place is a huge relief. I now have a robust monitoring system that will keep me informed about my EC2 instance’s health in real time. The log group provides a historical record of events, the alarm will notify me if anything goes wrong, and the dashboard allows me to quickly visualize the performance metrics.

In summary, I’ve created a fully integrated monitoring solution using AWS CloudWatch, with a log group for storing logs, an alarm to notify me if CPU utilization exceeds the threshold of 5%, and a dashboard to track performance. This system ensures my application runs smoothly and allows me to address potential issues before they impact users.

**output of the task**:

