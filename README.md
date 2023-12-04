# Problem Statement:

You're tasked with creating data storage solutions using Amazon EBS and EFS for different use cases.

## Guidelines/Goals:

### Amazon EBS Setup:

Create an Amazon EBS volume and attach it to an EC2 instance.
Format and mount the volume to a specific directory.
Use EBS for Application Data:

Create a simple text file on the EBS volume.
Ensure the data persists even if the instance is stopped and started.
Amazon EFS Setup:

### Amazon EBS Setup:

Create an Amazon EFS file system.
Mount the file system on multiple EC2 instances.
Use EFS for Shared Data:

Create a file on one instance and verify its presence on another.
Observe how changes to the file on one instance are reflected on the other.
Delete all created resources.

#### Amazon EFS Commands:
sudo yum -y update
mkdir ~/efs-mount-point

#### Install EFS utils:
sudo yum install -y amazon-efs-utils

#### Mount using the EFS mount helper:
sudo mount -t efs -o tls fs-07e81bffbc1ad1c53.efs.us-west-2.amazonaws.com:/ ~/efs-mount-point

#### Unmount the EFS file system:
sudo unmount ~/efs-mount-point

### Here is the PDF with [Steps Taken and Key Insights](https://github.com/olatunji-weber/aws-storage/blob/master/AWS%20Storage%20Project.pdf):
