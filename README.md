# Automated .NET Core HTTP Service Deployment on AWS

## Overview

is a lightweight **.NET 6 HTTP service** that runs on an AWS EC2 instance and serves random **Amazon S3 facts** with timestamps over HTTP.

The service is deployed **automatically** using a Bash script that:

- Installs all required dependencies (dotnet, git, AWS CLI).
- Clones source code from **AWS CodeCommit**.
- Builds and publishes the .NET service.
- Configures the service as a **systemd unit** so it runs in the background and restarts on reboot.

This project demonstrates **cloud automation**, **infrastructure as code**, and **continuous deployment practices** on AWS.

## Usage

Once deployed, access the service:

- curl http://<EC2-IP>:8002/

Example response:
15:42:31.1576890 - Protect your data with unmatched security, compliance, and audit capabilities.

## Learning Outcomes

- How to build lightweight HTTP services in C#

- How to automate deployments using Bash scripting

- How to integrate AWS CodeCommit with EC2

- How to manage background applications using systemd

- How to expose and test APIs in a cloud environment
