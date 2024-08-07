# Step 1: Install the AWS CLI in Ubuntu.

curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install

# Step 2: Configure the AWS CLI

    aws configure

Enter your AWS credentials and region:
You will be prompted to enter the following information:

    AWS Access Key ID: Your AWS access key.
    AWS Secret Access Key: Your AWS secret key.
    Default region name: The default region you want to use (e.g., us-west-2).
    Default output format: The output format (e.g., json, text, yaml, or table).

# Example:

bash

    AWS Access Key ID [None]: YOUR_ACCESS_KEY_ID
    AWS Secret Access Key [None]: YOUR_SECRET_ACCESS_KEY
    Default region name [None]: us-west-2
    Default output format [None]: json

# Step 3: Verify the Setup

Check the AWS CLI version:

    aws --version

This should display the version of the AWS CLI installed, confirming the installation was successful.

Verify AWS CLI configuration:

    aws sts get-caller-identity

This command returns details about your AWS account and verifies that the AWS CLI is configured correctly with your credentials.
