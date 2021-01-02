# Cloud Storage
-------------------------------------------------

We'll cover the following:
* [What is Block Storage?](#what-is-block-storage)
  - [Block Storage Use Cases](#block-storage-use-cases)
  - [Block Storage Options in the Cloud](#block-storage-options-in-the-cloud)
* [What is Object Storage?](#what-is-object-storage)
  - [Object Storage Use Cases](#object-storage-use-cases)
  - [Object Storage Options in the Cloud](#object-storage-options-in-the-cloud)
* [Conclusion](#conclusion)

Cloud Computing, like any computing, is a combination of CPU, memory, networking, and storage. 
**Infrastructure as a Service** (IaaS) platforms allow you to store your data in either Block Storage or Object 
Storage formats.

Understanding the differences between these **two formats** – and how they can sometimes be used 
together – can be a critical part of designing an overall storage profile. And the relatively low costs of 
[cloud storage](https://cloudacademy.com/amazon-web-services/aws-storage-fundamentals-aws-140-course/), 
along with its durability and high availability, can make it attractive even for local infrastructure projects.

## What is Block Storage?

**Block storage** devices provide fixed-sized raw storage capacity. Each storage volume can be treated as an 
independent disk drive and controlled by an external server operating system. This block device can 
be mounted by the guest operating system as if it were a physical disk. The most common examples of 
Block Storage are SAN, iSCSI, and local disks.

Block storage is the **most commonly used storage type** for most applications. It can be either locally or 
network-attached and are typically formatted with a file system like FAT32, NTFS, EXT3, and EXT4.

#### Block Storage Use Cases

* **Ideal for databases**, since DB requires consistent I/O performance and low-latency connectivity.
* Use block storage for **RAID Volumes**, where you combine multiple disks organized through stripping
  or mirroring.
* Any application which requires **server side processing**, like Java, PHP, and .Net will require block
  storage.
* Running **mission-critical** applications like Oracle, SAP, Microsoft Exchange, and Microsoft SharePoint.

#### Block Storage Options in the Cloud

1.  [AWS Elastic Block Storage (EBS)](https://cloudacademy.com/course/aws-storage-fundamentals-2016/amazon-elastic-block-store-ebs-1/): 
    Amazon EBS provides raw storage - just like a hard disk - which you can attach to your [Elastic Cloud Compute](https://cloudacademy.com/learning-paths/ec2-knowledge-assessment-62/) (EC2)
    instances. Once attached, you can create a file system and get immediate access to your storage. You can create 
    EBS General Purpose (SSD) and provisioned IOPS (SSD) volumes up to 16 TB in size, and slower, legacy magnetic 
    volumes.   
1.  **Rackspace Cloud Block Storage**: Rackspace provides raw storage devices capable of delivering super fast 10GbE 
    internal connections.
1.  **Azure Premium Storage**: [Premium Storage](https://cloudacademy.com/course/intro-to-azure-storage/) delivers 
    high-performance, low-latency disk support for I/O intensive workloads running on Azure Virtual Machines. 
    Volumes allow up to 32 TB of storage.
1.  **Google Persistent Disks**: [Compute Engine Persistent Disks](https://cloudacademy.com/learning-paths/google-cloud-platform-fundamentals-54/) 
    provide network-attached block storage, much like a high speed and highly reliable SAN, for Compute Engine 
    instances. You can remove a disk from one server and attach it to another server, or attach one volume to 
    multiple nodes in read-only mode. Two types of block storage are available: Standard Persistent Disk and 
    Solid-State Persistent Disks.

## What is Object Storage?

Block storage volumes can only be accessed when they’re attached to an operating system. But data kept 
on object storage devices, which consist of the object data and metadata, can be **accessed directly** 
**through APIs** or http/https. You can store any kind of data, photos, videos, and log files. The object store 
guarantees that the data will not be lost. Object storage data can be replicated across different data 
centers and offer simple web services interfaces for access.

A simple use case would see application developers who deal with large amounts of user-generated 
media, using object storage to **store unlimited media files**. As data stores scale to hundreds of terabytes 
and then into the petabyte range and beyond, object storage becomes even more attractive.

#### Object Storage Use Cases
* Storage of **unstructured data** like music, image, and video files.
* Storage for backup files, database dumps, and log files.
* Large data sets. Whether you’re storing pharmaceutical or financial data, or multimedia files such as 
  photos and videos, storage can be used as your **big data** object store.
* Archive files in place of local tape drives. Media assets such as **video footage** can be stored in object 
  storage and archived to [AWS glacier](https://cloudacademy.com/course/automated-data-management-with-ebs-s3-and-glacier/programmatically-accessing-glacier-via-java-apis-1/).

#### Object storage options in the Cloud
1.  **Amazon S3**: [Amazon S3](https://cloudacademy.com/course/automated-data-management-with-ebs-s3-and-glacier/setting-up-aws-s3-1/) stores data as objects within resources called “buckets.” AWS S3 offers 
    features like 99.999999999% durability, cross-region replication, event notifications, versioning, 
    encryption, and flexible storage options (redundant and standard).
1.  **Rackspace Cloud Files**: Cloud Files provides online object storage for files and media. Cloud Files 
    writes each file to three storage disks on separate nodes that have dual power supplies. All traffic 
    between your application and Cloud Files uses SSL to establish a secure, encrypted channel. You can 
    host static websites (for example: blogs, brochure sites, small company sites) entirely from Cloud Files 
    with a global CDN.
1.  **Azure Blob Storage**: For users with large amounts of unstructured data to store in the cloud, 
    [Blob storage](https://cloudacademy.com/course/intro-to-azure-storage/) offers a cost-effective and scalable 
    solution. Every blob is organized into a container with up to a 500 TB storage account capacity limit.
1.  **Google cloud storage**: Cloud Storage allows you to store data in Google’s cloud. 
    [Google Cloud Storage](https://cloudacademy.com/lab/working-google-cloud-storage-from-the-console/) supports 
    individual objects that are terabytes in size. It also supports a large number of buckets per account. 
    Google Cloud Storage provides strong read-after-write consistency for all upload and delete operations. 
    Two types of storage class are available: Standard Storage class and Storage Near line class (with Near Line 
    being **MUCH** cheaper).

## Conclusion

Object storage and Block storage both have **unique advantages and limitations**. Understanding the use 
cases and costs associated with each medium will help you get the best possible mileage out of your 
application storage profile.

:back:[**Back - Long-Polling vs WebSockets vs Server-Side Events**](../011_Long-Polling_vs_WebSockets_vs_Server-Side-Events/README.md)

### Progress Tracker

- [x] Mark as Completed
