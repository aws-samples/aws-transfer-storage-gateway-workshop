# Access data in Amazon S3 using AWS Transfer Family and AWS Storage Gateway

© 2020 Amazon Web Services, Inc. and its affiliates. All rights reserved.
This sample code is made available under the MIT-0 license. See the LICENSE file.

Errors or corrections? Contact [jeffbart@amazon.com](mailto:jeffbart@amazon.com).

---

## Workshop scenario

In many industries, organizations frequently need to exchange data with other parties.  This data is often encapsulated in reports stored in a well-known format.  Today, many organizations generate these reports internally and then make them available to external entities using common file transfer protocols such as SFTP.  In many cases, these reports must be preserved to meet compliance requirements, being stored in on-premises storage systems or in offsite vaults, often for many years.  In these types of workflows, organizations need to provide access to data both through standard file storage protocols such as NFS and SMB, as well as common file transfer protocols such as SFTP, FTP, or FTPS.

This workshop will show you how to use [AWS Transfer Family](https://aws.amazon.com/aws-transfer-family/) and [AWS Storage Gateway](https://aws.amazon.com/storagegateway/) to provide access to data from different file protocols.  Each of these services allows you to store and access data in [Amazon S3](https://aws.amazon.com/s3/) for scalable, durable cloud storage.

## Topics covered

- Deploying resources using CloudFormation
- Using AWS Storage Gateway to create and access files in Amazon S3 using NFS/SMB
- Using AWS Transfer Family to create and access data in Amazon S3 using SFTP/FTP/FTPS
- File Gateway RefreshCache API

## Prerequisites

#### AWS Account

In order to complete this workshop, you will need an AWS account with rights to create AWS IAM roles, EC2 instances, Storage Gateway shares, AWS Transfer servers, and CloudFormation stacks in the AWS regions you select.

#### Software

- **Internet Browser**  – It is recommended that you use the latest version of Chrome or Firefox for this workshop.

## Cost

It will cost approximately **3.00 USD** to run this workshop.  It is recommended that you follow the cleanup instructions once you have completed the workshop to remove all deployed resources and limit ongoing costs to your AWS account.

## Related workshops

- [NFS server migration using AWS DataSync and Storage Gateway](https://github.com/aws-samples/aws-datasync-migration-workshop/blob/master/workshops/nfs-migration)
- [IP whitelisting with AWS Transfer Family](https://github.com/aws-samples/aws-transfer-sftp-ip-whitelisting-workshop)

## Workshop modules

This workshop consists of the following modules:

- [Module 1](/module1) - Deploy resources using CloudFormation
- [Module 2](/module2) - Configure the File Gateway
- [Module 3](/module3) - Configure the AWS Transfer server
- [Module 4](/module4) - Using RefreshCache to see changes in S3
- [Module 5](/module5) - Cleanup resources

To get started, go to [Module 1](/module1).
