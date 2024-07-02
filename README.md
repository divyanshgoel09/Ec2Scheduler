# Ec2Scheduler
Some organizations only need their EC2 instances during specific hours, such as from 10:00 AM to 12:00 PM (You can set time according to youyr need). To manage this, I will create two Lambda functions to start and stop the instances. These functions will be triggered by CloudWatch Events scheduled for the morning and evening, providing a fully serverless solution.

![image](https://github.com/divyanshgoel09/Ec2Scheduler/assets/118998853/173af1d6-e004-44b9-aae0-078fbc521a65)

A EC2 instance which will get start and stop on fix time in a day 
![image](https://github.com/divyanshgoel09/Ec2Scheduler/assets/118998853/db7fa4a0-9311-4352-b720-1aa83353891c)

Some policies which will be used for start and stop 
![image](https://github.com/divyanshgoel09/Ec2Scheduler/assets/118998853/2ccd73d4-efd8-4039-b352-b84fb537c892)

We created two Lambda Function to trigger start and stop 

START
![image](https://github.com/divyanshgoel09/Ec2Scheduler/assets/118998853/c95154b7-40a4-4248-8a06-e7fab2b0cec3)

STOP
![image](https://github.com/divyanshgoel09/Ec2Scheduler/assets/118998853/3718cc4c-4879-463d-be6d-3e43275c156a)

We attached Start and Stop policies to respective La,bda Function

Now we created Event Scheduler 
![3](https://github.com/divyanshgoel09/Ec2Scheduler/assets/118998853/eb182181-43b0-4adb-95df-a2f309cdb8ef)
![4](https://github.com/divyanshgoel09/Ec2Scheduler/assets/118998853/972d9961-48b4-4237-b2d7-c3db1a5f184c)

![2](https://github.com/divyanshgoel09/Ec2Scheduler/assets/118998853/502a2107-4457-42ab-bc0c-1a6ba3e84cc4)

User Receives AWS notification at scheduled start and stop time by the SNS service on AWS.

