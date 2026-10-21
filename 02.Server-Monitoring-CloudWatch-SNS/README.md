# AWS Server Monitoring with CloudWatch and SNS

## Project Overview

This project demonstrates how to implement server monitoring and automated alerting using Amazon CloudWatch and Amazon Simple Notification Service (SNS).

The solution continuously monitors the health and performance of an Amazon EC2 instance and sends notifications when predefined thresholds are exceeded. This helps improve operational visibility and enables rapid response to potential issues.

## Business Requirement

Organizations need a monitoring solution that:

- Detects performance issues early
- Provides real-time visibility into server health
- Automatically alerts administrators
- Reduces system downtime
- Improves operational efficiency

## AWS Services Used

- Amazon EC2
- Amazon CloudWatch
- Amazon SNS
- AWS IAM

## Solution Architecture

EC2 Instance → CloudWatch Metrics → CloudWatch Alarm → SNS Topic → Email Notification

## Components

### Amazon EC2

Hosts the application or workload being monitored.

### Amazon CloudWatch

Collects and monitors performance metrics including:

- CPU Utilization
- Network Activity
- Disk Performance
- System Health Metrics

### CloudWatch Alarms

Configured to monitor specific thresholds and trigger actions when conditions are met.

### Amazon SNS

Delivers notifications to administrators when alarms are triggered.

### IAM

Provides secure access control and permissions management.

## Implementation Steps

1. Launch an Amazon EC2 instance.
2. Configure CloudWatch monitoring.
3. Create an SNS topic.
4. Subscribe an email address to the SNS topic.
5. Confirm the SNS subscription.
6. Create CloudWatch alarms.
7. Define threshold values.
8. Associate alarms with the SNS topic.
9. Generate test activity to trigger alarms.
10. Verify email notification delivery.

## Monitoring Scenario

A CloudWatch alarm monitors EC2 CPU utilization.

When CPU usage exceeds the configured threshold:

1. CloudWatch detects the condition.
2. The alarm changes state.
3. SNS receives the event.
4. An email notification is sent.
5. The administrator is alerted and can investigate.

## Skills Demonstrated

- AWS Monitoring and Observability
- CloudWatch Metrics and Alarms
- SNS Notification Services
- EC2 Administration
- Incident Detection
- Operational Excellence
- AWS Security and IAM
- Troubleshooting and Alerting

## Challenges and Lessons Learned

### Challenge

Configuring alarm thresholds that provide meaningful alerts without generating unnecessary notifications.

### Solution

Carefully selected threshold values and tested alarm conditions before deployment.

### Key Learning

Monitoring and alerting are critical components of cloud operations and help teams proactively identify and resolve issues before they impact users.

## Security Considerations

- Principle of least privilege applied through IAM.
- Controlled access to monitoring resources.
- Secure notification delivery through verified SNS subscriptions.

## Future Improvements

- Add CloudWatch Dashboards.
- Monitor additional custom metrics.
- Integrate with AWS Lambda for automated remediation.
- Configure multi-channel alerting.
- Implement centralized logging using CloudWatch Logs.

## Project Outcome

Successfully implemented a monitoring and alerting solution using Amazon CloudWatch and Amazon SNS. The project demonstrated how AWS services can be combined to improve operational visibility, automate notifications, and support proactive system management.
