# Purpose

**Work-In-Progress**

ec2SpotNotify is aimed to monitor EC2 Instance Metadata for EC2 Spot Termination Notices every 3 seconds. Once termination notice has been provided by EC2, you can run an arbitrary command or send a message to AWS SNS in which you can invoke a Lambda function thereafter (i.e resize AutoScaling Group for on-demand instances, send to SQS queue and count it later, etc).

## Why yet another EC2 Spot SNS small program?

I'm actually using it for the sake of learning Go more appropriately, so nothing better than having small projects as I have bigger ones to come :)

# Platform supported

This program should be able to run in both Linux and Windows platforms. 

# Deployment

[!] TODO

# TODO
* Create Golang package and organize files
* Create test for package

## Improvements
* Make comments 'godoc' compatible so it can generate HTML if needed
* Read TimeThresholdTime from Config file instead of const for more flexibility
* Generate builds for Linux and Windows
* Write quick start guide for both Linux and Windows including IAM SNS Permissions for EC2 IAM Role