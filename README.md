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
3. To confirm the installation, open a command prompt window, and at the command prompt use the aws --version command.
   ```
   aws --version
   ```
5. Refresh the command prompt window to check, if you dont see te version details.
