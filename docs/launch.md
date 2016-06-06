

## Getting Started

Use the instructions below to launch a **cloud controller**. Once created,
you can use the controller to spin-up, use and spin-down one or more clusters.

> There is an option to launch the **cloud controller** and a single **cluster** together (i.e. "Quick Launch").
Refer to [Cluster Quick Launch](quick.md) for more information.


## Setup Prerequisites

1. Review the Hortonworks Cloud [Terms of Use](terms.md).

2. Setup AWS Account. If you already have an AWS account, login to the [AWS
Management Console](http://aws.amazon.com). Alternatively, you can create a new AWS account following the
instructions provided by AWS.

3. Setup key pair. The Amazon EC2 instances that you create 
will be accessible by the key pair you provide during installation. Refer to
the [AWS documentation](http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-key-pairs.html#having-ec2-create-your-key-pair)
for instructions on how to create a key pair. 

## Launching the Cloud Controller

1. We provide a CloudFormation template to create the AWS resources and EC2 Instance to run the cloud controller. Click to launch the <a href="https://console.aws.amazon.com/cloudformation/home?region=eu-central-1#/stacks/new?stackName=HortonworksCloud&templateURL=https://s3-eu-west-1.amazonaws.com/cloudbreak-cloudformation/cbd-advanced-0.1.template" target="_blank">CloudFormation template</a>.

2. Click **Next**. The **Specify Details** page is shown.

3. Enter the following **Parameters**.

    | Parameter| Description|
    |---|---|
    |SSH Key Name|Name of an existing EC2 key pair to enable SSH to access the instances|
    |VPC|PLACEHOLDER|
    |Remote Location|Enter the CIDR mask to allow for remote access. For example 0.0.0.0/0 allows for full access. |
    |Admin Username|Enter an email address to use as the admin username. |
    |Admin Password|Enter the admin password. Minimum 8 characters with at least 1 uppercase, 1 numeric and 1 special character. |

4. Click **Next**. The **Options** page is shown.

5. Click **Next**. The **Review** page is shown.

6. Click the **I acknowledge** checkbox and click **Create**.

    > The **Stack Name** is shown in the table with a CREATE_IN_PROGRESS **Status**. The create process
    can take a few minutes and once ready, you will see CREATE_COMPLETE.

7. Once complete, browse instance created at the **CloudbreakURL** provided in the **Outputs**. 

## Log In

1. Browse to cloud controller instance created.

2. Log in using the Admin Username and Password provided during the controller launch.

3. On first login, you will be prompted to accept the [Terms of Use](terms.md) to continue.

4. Once accepted, you will be shown the Hortonworks Cloud UI.

![Hortonworks Cloud](/cloud-ui.png)
