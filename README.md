# AWS-IAM-CloudFormation-Automation-Lab
This lab demonstrates how to automate the creation of IAM Users and Roles in AWS using CloudFormation. You will follow the Principle of Least Privilege, verify resource creation, and clean up your environment at the end.



Step 1: Sign in to AWS Console
Log in to your AWS account as the IAM admin user (admin-student). Ensure you are not using the root account.
Screenshot #1: AWS Console home page showing your admin-student username.

![User List](screenshots/Screenshot%202025-10-06%20164416.png)
![Admin Student](screenshots/Screenshot%202025-10-06%20170159.png
)



Step 2: Open CloudFormation Service
Navigate to the CloudFormation service and start creating a new stack.
Screenshot #2: CloudFormation 'Create Stack' setup screen.

Screenshot(s): _______________________________



Step 3: Upload the Template File
Upload the iam-template.yaml file that defines your IAM resources.
Screenshot #3: Confirmation of uploaded YAML file.

Screenshot(s): _______________________________



Step 4: Create the Stack
Name your stack Student-IAM-Lab and deploy it.
Screenshot #4: CREATE_IN_PROGRESS status.
Screenshot #5: CREATE_COMPLETE status.

Screenshot(s): _______________________________



Step 5: Verify IAM Resources
Check IAM → Roles for StudentLabRole and IAM → Users for StudentLabUser.
Screenshot #6: CloudFormation Resources tab.
Screenshot #7: StudentLabRole policy.
Screenshot #8: StudentLabUser policy.

Screenshot(s): _______________________________



Step 6: Test Least Privilege (Optional but Recommended)
Create a password for StudentLabUser, log in, and test access to S3 (allowed) and IAM (denied).
Screenshot #9: StudentLabUser AWS Console login.
Screenshot #10: Access Denied message in IAM.

Screenshot(s): _______________________________



Step 7: Clean Up Resources
Delete the CloudFormation stack to remove all created resources.
Screenshot #11: DELETE_COMPLETE confirmation.

Screenshot(s): _______________________________


