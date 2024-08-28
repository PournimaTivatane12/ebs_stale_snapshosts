# AWS Cloud Cost Optimization - Identifying Stale Resources

# Identifying Stale EBS Snapshots

In this example, we'll create a Lambda function that identifies EBS snapshots that are no longer associated with any active EC2 instance and deletes them to save on storage costs.

Description:
The Lambda function fetches all EBS snapshots owned by the same account ('self') and also retrieves a list of active EC2 instances (running and stopped). For each snapshot, it checks if the associated volume (if exists) is not associated with any active instance. If it finds a stale snapshot, it deletes it, effectively optimizing storage costs.

This project focuses on identifying and cleaning up stale snapshots in the Amazon Elastic Block Store (EBS). By leveraging AWS cloud skills, the goal is to automate the detection of old, unused snapshots, reducing unnecessary costs and ensuring efficient cloud resource management.

Features:

1. Automated detection of stale EBS snapshots based on customizable criteria (e.g., age, tags).

2. Integrated cleanup process to delete unused snapshots safely.

3. Uses AWS SDK and Lambda for automation.

4. Detailed logging for audit and monitoring purposes.

5. Easy deployment with Terraform or CloudFormation templates.

![image](https://github.com/user-attachments/assets/0d61d10b-3ade-4fc7-a17c-77f4cf7fd981)

![image](https://github.com/user-attachments/assets/a6436a7a-e56e-46b9-b208-3cf91f7fc036)

![image](https://github.com/user-attachments/assets/352d9777-b8f3-4bda-b41d-d6d134709369)



