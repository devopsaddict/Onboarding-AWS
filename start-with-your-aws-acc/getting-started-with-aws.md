# Starting with AWS account creation and setup

## Create an IAM user in your AWS account

1. You can create the in management console [CreateUser in Management Console](https://docs.aws.amazon.com/IAM/latest/UserGuide/getting-started-workloads.html)
2. You can also create IAM user with AWS CLI
     ```
      aws iam create-user --user-name Automation
     ```
4. Create an IAM user group named AutomationGroup, attach the AWS managed policy PowerUserAccess to the group, and then add the Automation user to the group
     * Create AWS IAM Group
          ```
           aws iam create-group --group-name AutomationGroup
          ```
     * Iam Attach group policy
          ```
           aws iam attach-group-policy --policy-arn arn:aws:iam::aws:policy/PowerUserAccess --group-name AutomationGroup
          ```
     * Iam add user to the group
         ```
          aws iam add-user-to-group --user-name Automation --group-name AutomationGroup
         ```
     * Run the aws iam get-group command to list the AutomationGroup and its members
         ```
          aws iam get-group --group-name AutomationGroup
         ```
4. Create access credentials for the required workloads
     *  Creating access keys for the user
         ```
          aws iam create-access-key --user-name Automation
         ```
              
               
