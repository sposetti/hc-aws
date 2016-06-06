
## Creating a Cluster

1. Browse to your running Hortonworks Cloud controller instance and Log In.

1. Click **CREATE CLUSTER**.

2. For **GENERAL CONFIGURATION**, enter the following parameters.

    | Parameter| Description|
    |---|---|
    |Cluster Name|Enter the name for this cluster.|
    |HDP Version|Enter the name for this cluster.|
    |Cluster Type|Choose the type of cluster. See [Cluster Type](architecture/#cluster-types) for more information. |

3. For **HARDWARE**, the default options allow you to select the Instance Type for all Nodes and Count for Worker Nodes

    | Parameter| Description|
    |---|---|
    |Instance Type|Choose the instance type for all nodes (Master and Worker).|
    |Instance Count|Enter the number of Worker nodes. The cluster will be created with 1 Master and this number of Worker nodes.|

    You can expand to *SHOW ADVANCED OPTIONS* for more granular control of instances and storage.

    | Parameter| Description|
    |---|---|
    |Master Instance Type|Choose the instance type for the Master node.|
    |Worker Instance Type|Choose the instance type for the Worker nodes.|
    |Instance Count|Enter the number of Worker nodes. The cluster will be created with 1 Master and this number of Worker nodes.|
    |Storage|TBD|

3. For **NETWORK & SECURITY**, the default options allow you to select the Instance Type for all Nodes and Count for Worker Nodes

    | Parameter| Description|
    |---|---|
    |SSH Key Name|Name of an existing EC2 key pair to enable SSH to access the cluster instances. |
    |Remote Location|Enter the CIDR mask to allow for remote access. For example **0.0.0.0/0** will allow for full access. |
    |Web Access| Check this option to provide open access to the cluster Web UI ports. |
     
    You can expand to *SHOW ADVANCED OPTIONS* for additional options.

    | Parameter| Description|
    |---|---|
    |Instance Role | TBD |

3. Click **CREATE CLUSTER**.