Preparing CloudFormation storage

After we create three CloudFormation files for testing and production stages, we should
prepare a storage for our CloudFormation template files. For demo, we use Amazon S3
bucket.
Next, we perform the following tasks:
Creating Amazon S3 bucket
Uploading CloudFormation template files
Creating Amazon S3 bucket
We need Amazon S3 bucket to store our template files so CloudFormation can download
these template files and perform provisions.
You can follow these steps to create Amazon S3 bucket:
1. Open a browser and navigate to https://s3.console.aws.amazon.com/s3/home.
2. You should log in with your active account.
3. If succeed, you should get Amazon S3 dashboard as shown in the following
4. Click on the + Create bucket button.
5. You should get a dialog as shown in the following screenshot. Fill all required
fields. If done, click the Next button:
6. Then, you should get a form as shown in the following screenshot. Check
the Versioning option. If done, click the Next button:
7. You will be asked to review all entries. Click Create to complete all tasks. After
created, you should see your Amazon S3 bucket, for instance, lambacloud, as
shown in the following screenshot:
Uploading CloudFormation template files
We can upload our compress template file. For demo, we upload lambda.zip file:
1. Open Amazon S3 Bucket that we already created
2. Click the Upload button and select lambda.zip file.
3. If succeed, we can see our lambda.zip file on Amazon S3 bucket as shown in
the following screenshot:
Configuring AWS IAM
Since we make interaction with AWS CodePipeline from AWS CloudFormation, we should
configure our AWS users that access AWS CloudFormation.
This is done if we use AWS IAM. You can open AWS IAM using browser and navigate
to https://console.aws.amazon.com/iam/home. Attach the AWSCodePipelineFullAccess
policy into your account or role. You can see the AWSCodePipelineFullAccess policy in
the following screenshot: