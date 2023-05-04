# Resume Sync to AWS CodeCommit

Set up an AWS CodeCommit repository:

- Sign in to the AWS Management Console and open the AWS CodeCommit console at https://console.aws.amazon.com/codecommit/.
- Click "Create repository" and follow the instructions to create a new repository.

Create an IAM user with AWS CodeCommit permissions:
- Open the IAM console at https://console.aws.amazon.com/iam/.
- Create a new user 
- Attach the "AWSCodeCommitPowerUser" managed policy from the "Attach policies directly" dropdown.
- Create user, then click on username, security credentials.
- Grant programmatic access.
- Save the access key ID and secret access key for later use.

Add the IAM user's AWS access key and secret access key as GitHub repository secrets:
- Go to your GitHub repository's "Settings" and click on "Secrets".
- Click "New repository secret" and add two secrets, "AWS_ACCESS_KEY_ID" and "AWS_SECRET_ACCESS_KEY", with the values obtained in step 2.