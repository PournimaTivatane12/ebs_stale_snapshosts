1. AWS Account

An active AWS account with necessary permissions to manage EBS snapshots.

AWS IAM user/role with the following permissions:

ec2:DescribeSnapshots

ec2:DeleteSnapshot

ec2:DescribeVolumes

2. AWS CLI

Install the AWS Command Line Interface (CLI) on your local machine.

Configure it with your AWS credentials:

aws configure

3. Python Environment

Python 3.x installed on your system.

Required dependencies (install using pip):

pip install boto3

4. IAM Role (For Lambda Execution)

If deploying as an AWS Lambda function, ensure:

The Lambda function has an IAM role with permissions to manage EBS snapshots.

Attach a policy with AmazonEC2ReadOnlyAccess and ec2:DeleteSnapshot permissions.

5. Logging & Monitoring

Enable AWS CloudWatch logs for debugging and monitoring stale snapshot deletion activities.

6. Deployment Options

Run the script locally or deploy it as a Lambda function.

If using Lambda, package the dependencies and upload the zip file.

7. Optional: Terraform Setup

If you prefer infrastructure as code (IaC), you can define resources in Terraform.

Once these prerequisites are met, proceed with configuring and running the script as per the project documentation.

