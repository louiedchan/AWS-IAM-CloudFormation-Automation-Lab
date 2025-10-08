# AWS-IAM-CloudFormation-Automation-Lab
This lab demonstrates how to automate the creation of IAM Users and Roles in AWS using CloudFormation. You will follow the Principle of Least Privilege, verify resource creation, and clean up your environment at the end.



Step 1: Sign in to AWS Console
Log in to your AWS account as the IAM admin user (admin-student). Ensure you are not using the root account.
Screenshot #1: AWS Console home page showing your admin-student username.

![User List](screenshots/Screenshot%202025-10-06%20164416.png)
![Admin Student](screenshots/Screenshot%202025-10-06%20170159.png
)


Step 2 & 3: Open CloudFormation Service and Upload the Template File
Navigate to the CloudFormation service and start creating a new stack.
Upload the iam-template.yaml file that defines your IAM resources.
Screenshot #2: CloudFormation 'Create Stack' setup screen and Confirmation of uploaded YAML file.

![Stack](screenshots/Screenshot%202025-10-06%20171345.png)

Step 4: Create the Stack
Name your stack Student-IAM-Lab and deploy it.
Screenshot #4: CREATE_IN_PROGRESS status.
![InProgress](screenshots/Screenshot%202025-10-06%20171516.png)
Screenshot #5: CREATE_COMPLETE status.
![Complete](screenshots/Screenshot%202025-10-06%20172043.png)


Step 5: Verify IAM Resources
Check IAM → Roles for StudentLabRole and IAM → Users for StudentLabUser.

Screenshot #6: StudentLabRole policy.
![LabRole](screenshots/Screenshot%202025-10-06%20172242.png)

Screenshot #7: StudentLabUser policy.
![LabUser](screenshots/Screenshot%202025-10-06%20172320.png)





Step 6: Test Least Privilege (Optional but Recommended)
Create a password for StudentLabUser, log in, and test access to S3 (allowed) and IAM (denied).
Screenshot #9: StudentLabUser AWS Console login.
![ConsoleLogin](screenshots/Screenshot%202025-10-06%20174319.png)
Screenshot #10: Access Denied message in IAM.
![Access](screenshots/Screenshot%202025-10-06%20175542.png)



Step 7: Clean Up Resources
Delete the CloudFormation stack to remove all created resources.
Screenshot #11: DELETE_COMPLETE confirmation.

Screenshot(s): _______________________________


