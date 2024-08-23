AWS Cloud Cost Optimization - Identifying Stale Resources
Identifying Stale EBS Snapshots
In this example, we'll create a Lambda function that identifies EBS snapshots that are no longer associated with any active EC2 instance and deletes them to save on storage costs.

Description:
The Lambda function fetches all EBS snapshots owned by the same account ('self') and also retrieves a list of active EC2 instances (running and stopped). For each snapshot, it checks if the associated volume (if exists) is not associated with any active instance. If it finds a stale snapshot, it deletes it, effectively optimizing storage costs.

This project focuses on identifying and cleaning up stale snapshots in the Amazon Elastic Block Store (EBS). By leveraging AWS cloud skills, the goal is to automate the detection of old, unused snapshots, reducing unnecessary costs and ensuring efficient cloud resource management.

Features:

Automated detection of stale EBS snapshots based on customizable criteria (e.g., age, tags).
Integrated cleanup process to delete unused snapshots safely.
Uses AWS SDK and Lambda for automation.
Detailed logging for audit and monitoring purposes.
Easy deployment with Terraform or CloudFormation templates.

![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/d814276b-80aa-4aa6-9d93-6a2eb4ca7eec/bdf0e324-aa18-4f7d-bfa4-fb0291aa3253/image.png)
