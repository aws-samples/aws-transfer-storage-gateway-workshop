# Access data in Amazon S3 using AWS Transfer Family and AWS Storage Gateway

© 2020 Amazon Web Services, Inc. and its affiliates. All rights reserved.
This sample code is made available under the MIT-0 license. See the LICENSE file.

Errors or corrections? Contact [jeffbart@amazon.com](mailto:jeffbart@amazon.com).

---

# Module 5
## Workshop clean-up

To make sure all resources are deleted after this workshop scenario make sure you execute the steps in the order outlined below (you do not need to wait for CloudFormation to finish deleting before moving to the next step):

1. Unmount the File Gateway NFS share on the Linux server by running the following command:

        $ sudo umount /mnt/nfs

2. Close the browser window running the CLI.
3. Go to the Storage Gateway page in the AWS console and delete the **NFS file share**.
4. On the left side of the Storage Gateway console, click on **Gateways** and delete the File Gateway named **WorkshopGateway**.  Note that this will not delete the gateway EC2 instance itself.  The instance will get deleted when the CloudFormation stack is deleted.
5. Delete all objects in the S3 bucket that was created for this workshop.  The bucket must be empty before it can be deleted by CloudFormation in the next step.
5. Go to the CloudFormation page and delete the stack named **TransferWorkshop**.  It will take a few minutes for the stack to be fully deleted.

To make sure that all CloudFormation templates have been deleted correctly, confirm that any EC2 instances created in this workshop are in the **terminated** state.
