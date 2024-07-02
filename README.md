# Ec2Scheduler
Some organizations only need their EC2 instances during specific hours, such as from 8:00 AM to 5:00 PM. To manage this, I will create two Lambda functions to start and stop the instances. These functions will be triggered by CloudWatch Events scheduled for the morning and evening, providing a fully serverless solution.
