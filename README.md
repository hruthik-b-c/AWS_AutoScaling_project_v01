# AWS EC2 Auto Scaling Project

This project demonstrates real-world implementation of EC2 Auto Scaling
using Launch Templates, Application Load Balancer, and Target Tracking.

## Architecture
- EC2 Launch Template
- Auto Scaling Group (Min 1, Desired 2, Max 5)
- Application Load Balancer
- Target Group
- CloudWatch Metrics

## Scaling Policy
- Metric: Average CPU Utilization
- Target value: 5%
- Automatic scale-in and scale-out

## Validation
CPU stress test performed using:
stress --cpu 2 --timeout 300

## Outcome
- Automatic scale-out on CPU spike
- High availability across AZs
- Zero manual intervention
