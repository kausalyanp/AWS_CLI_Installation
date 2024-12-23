# Step by step Guild to Install AWS CLI in Windows.

1. Download and run the AWS CLI MSI installer for Windows (64-bit):
https://awscli.amazonaws.com/AWSCLIV2.msi

2. Alwternative Steps:
     1. Run the msiexec command to run the MSI installer.
        ```
        msiexec.exe /i https://awscli.amazonaws.com/AWSCLIV2.msi
        ```
    2. Use the /qn flag for a silent installation
        ```
        msiexec.exe /i https://awscli.amazonaws.com/AWSCLIV2.msi /qn
        ```
3. To confirm the installation, open a command prompt window, change the directory to downloads.(or wherever your file present) and at the command prompt use the aws --version command.
   ```
   aws --version
   ```
5. Refresh the command prompt window to check, if you dont see te version details.

## Set New IAM User (Recomonded)
1. Create a new User
2. Give the adminstrator access
3. Connect the new user with AWS using Access key.

## Creating Access Key
1. Select your user in IAM,
2. Go to Create Access key section.
3. Choose, Command Line Interface (CLI)
4. Access key and Secret Access key will be generated for the user.
5. Now, from your command prompt. change directory to downloads and type-
   ```
   aws configure
   ```
6. Then fill all these details.
        1.AWS Access Key ID [None]: (enter your access key)
        2.AWS Secret Access Key [None]: (enter your secret access key)
        3. Default region name [None]:  (enter your region like us-east-1)
        4.Default output format [None]: (can be left empty, or enter json)
7. Now check if the AWS is connected with your AWS account using command- This command checks for the any s3 bucket present in your account.Create a bucket in advance.
   ```
   aws s3 ls
   ```


