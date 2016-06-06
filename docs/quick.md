

## Quick Launch

There is an option to launch the **cloud controller** and the **cluster** together (a "Quick Launch").
This is a typical DevOps scenario where you want to spin-up the cluster, use it and spin-down
the cluster and you do not plan to keep the **cloud controller** running.

1. Click to launch the <a href="https://console.aws.amazon.com/cloudformation/home?region=eu-central-1#/stacks/new?templateURL=https://s3-eu-west-1.amazonaws.com/cloudbreak-cloudformation/cbd-quick-0.1.template" target="_blank">CloudFormation template</a>.
2. Click **Next**. The **Specify Details** page is shown.
3. Enter the following **Parameters**.

    | Parameter| Description|
    |---|---|
    |SSH Key Name|Name of an existing EC2 key pair to enable SSH to access the instances.|
    |VPC|PLACEHOLDER|
    |Remote Location|Enter the CIDR mask to allow for remote access. For example 0.0.0.0/0 allows for full access. |
    |Admin Username|Enter an email address to use as the admin username. |
    |Admin Password|Enter the admin password that has at least 8 characters long with at least 1 uppercase, 1 numeric and 1 special character. |

4. Click **Next**. The **Options** page is shown.
5. Click **Next**. The **Review** page is shown.
6. Click the **I acknowledge** checkbox and click **Create**.

     > The **Stack Name** is shown in the table with a CREATE_IN_PROGRESS **Status**. The create process
     can take a few minutes and once ready, you will see CREATE_COMPLETE.

7. Cluster is ready to use.