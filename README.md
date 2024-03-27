# AWS CLI ESSENTIALS


## Prerequisites
- AWS account
- AWS CLI installed and configured
- Basic familiarity with AWS services

## Getting Started
1. **Create a Key Pair:**
   - Generate a key pair either through the AWS CLI or AWS Management Console to securely access EC2 instances.

2. **Create IAM User:**
   - Set up an IAM user with programmatic access and necessary permissions (e.g., EC2, S3) using AWS Management Console.

3. **Configure AWS CLI:**
   - Open a terminal or command prompt.
   - Run `aws configure` and provide your access key, secret key, default region (e.g., `ap-south-1` for Mumbai), and output format.

4. **Start EC2 Instance:**
   - Launch an EC2 instance using the command:
     ```
     aws ec2 run-instances --image-id AMI_ID --count 1 --instance-type INSTANCE_TYPE --key-name forawscli --region ap-south-1
     ```

5. **Manage Instances:**
   - Describe instances:
     ```
     aws ec2 describe-instances --region ap-south-1
     ```
   - Terminate instances:
     ```
     aws ec2 terminate-instances --instance-ids INSTANCE_ID --region ap-south-1
     ```


     ```


