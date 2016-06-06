
## Introduction

**Hortonworks Connected Data Cloud** (Hortonworks Cloud) is a system for launching and
managing a data lake on Amazon Web Services (AWS). Using Hortonworks Cloud, you can launch
clusters for analyzing and processing data with Apache Hadoop, Apache Hive and Apache Spark
powered by the <a href="http://hortonworks.com/products/hdp/" target="_blank">Hortonworks Data Platform</a>.

> Note: You are responsible for AWS charges while running Hortonworks Cloud and the clusters
being managed by Hortonworks Cloud.


## Prerequisites

To use Hortonworks Cloud, you need the following:

- **Amazon Web Services Account.** If you already have an AWS account, login to the [AWS
Management Console](http://aws.amazon.com). Alternatively, you can create a new AWS account following the
instructions provided by AWS.
- **Amazon Key Pair in your AWS Account.** The Amazon EC2 instances that you create for Hortonworks Cloud
will be accessible by the key pair you provide during installation. Refer to
the [AWS documentation](http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-key-pairs.html#having-ec2-create-your-key-pair)
for instructions on how to create a key pair. 

## AWS Services

The following AWS services are used by Hortonworks Cloud:

- Amazon EC2
- Amazon S3
- Amazon VPC
- AWS Lambda
- AWS CloudFormation
- Identity & Access Management