# Session-3-Assignment-1
MAJOR COMPONENTS OF HADOOP 2.X ARE: 1.Yarn 2.HDFS 3.Mapreduce

Yarn(Yet Another Resource Negotiator): Hadoop 2.x Architecture has one extra and new component that is : YARN. It is really game changing component in BigData Hadoop System. It is new Component in Hadoop 2.x Architecture. It is also know as “MR V2”.
i. Resource Manager (RM)
It is the master daemon of Yarn. It manages the global assignments of resources (CPU and memory) among all the applications. It arbitrates system resources between competing applications. follow this Hadoop yarn Resource Manager guide to learn Yarn Resource manager in great detail.

Resource Manager has two Main components

Scheduler

Application manager

a. Scheduler

The scheduler is responsible for allocating the resources to the running application. The scheduler is pure scheduler it means that it performs no monitoring no tracking for the application and even doesn’t guarantees about restarting failed tasks either due to application failure or hardware failures.

b. Application Manager
It manages running Application Masters in the cluster, i.e., it is responsible for starting application masters and for monitoring and restarting them on different nodes in case of failures.

ii. Node Manager (NM)
It is the slave daemon of Yarn. NM is responsible for containers monitoring their resource usage and reporting the same to the ResourceManager. Manage the user process on that machine. Yarn NodeManager also tracks the health of the node on which it is running. The design also allows plugging long-running auxiliary services to the NM; these are application-specific services, specified as part of the configurations and loaded by the NM during startup.

iii. Application Master (AM)
One application master runs per application. It negotiates resources from the resource manager and works with the node manager. It Manages the application life cycle.

The AM acquires containers from the RM’s Scheduler before contacting the corresponding NMs to start the application’s individual tasks.
Hadoop 2.x YARN has the following benefits.

1.Highly Scalability 2.Highly Availability : • There is a pair of NameNodes in an active-standby configuration • In the event of failure of an active NameNode, the standby takes over its duties without a significant interruption.

3.Supports Multiple Programming Models 4.Supports Multi-Tenancy 5.Supports Multiple Namespaces 6.Improved Cluster Utilization 7.Supports Horizontal Scalability

HDFS: HDFS stands for Hadoop Distributed File System. It is also know as HDFS V2 as it is part of Hadoop 2.x with some enhanced features. It is used as a Distributed Storage System in Hadoop Architecture.

Mapreduce: Map Reduce is a Batch Processing or Distributed Data Processing Module. It is also know as “MR V1” as it is part of Hadoop 1.x with some updated features.
