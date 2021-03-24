# Big-Data

Hadoop Mainly works on 3 Deployment Models
1. Standalone                  [Clientside only]
2. Psudo Distributed MOde      [Single Node]
3. Fully Distributed MOde      [Multi-Node]

![image](https://user-images.githubusercontent.com/21120537/112365942-3e50da00-8cfe-11eb-8e80-29d227f36e65.png)

1. Standalone Mode
In Standalone Mode none of the Daemon will run i.e. Namenode, Datanode, Secondary Name node, Job Tracker, and Task Tracker. We use job-tracker and task-tracker for processing purposes in Hadoop1. For Hadoop2 we use Resource Manager and Node Manager. Standalone Mode also means that we are installing Hadoop only in a single system. By default, Hadoop is made to run in this Standalone Mode or we can also call it as the Local mode. We mainly use Hadoop in this Mode for the Purpose of Learning, testing, and debugging.

2. Pseudo Distributed Mode (Single Node Cluster)
In Pseudo-distributed Mode we also use only a single node, but the main thing is that the cluster is simulated, which means that all the processes inside the cluster will run independently to each other. All the daemons that are Namenode, Datanode, Secondary Name node, Resource Manager, Node Manager, etc. will be running as a separate process on separate JVM(Java Virtual Machine) or we can say run on different java processes that is why it is called a Pseudo-distributed.
  Hadoop is used for development and for debugging purposes both.
  Our HDFS(Hadoop Distributed File System ) is utilized for managing the Input and Output processes.
  We need to change the configuration files mapred-site.xml, core-site.xml, hdfs-site.xml for setting up the environment.
  ![image](https://user-images.githubusercontent.com/21120537/112366404-c7681100-8cfe-11eb-981a-8c9aa0e9b708.png)

3. Fully Distributed Mode (Multi-Node Cluster)
This is the most important one in which multiple nodes are used few of them run the Master Daemon’s that are Namenode and Resource Manager and the rest of them run the Slave Daemon’s that are DataNode and Node Manager. Here Hadoop will run on the clusters of Machine or nodes. Here the data that is used is distributed across different nodes. This is actually the Production Mode of Hadoop let’s clarify or understand this Mode in a better way in Physical Terminology.
![image](https://user-images.githubusercontent.com/21120537/112366474-dbac0e00-8cfe-11eb-8410-2af373a8bc71.png)

