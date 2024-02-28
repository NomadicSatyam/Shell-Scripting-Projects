## Prerequisites

- Basic knowledge of AWS services.
- An AWS account with necessary permissions.

## Setup Steps

### Step 1: IAM Configuration

- Create a user ( give user name ) `eks-admin` with `AdministratorAccess`.
- Administrator Access has full access so choose this option change access type according to your requrement
- Generate Security Credentials: Access Key and Secret Access Key For Command Line InterFace.

### Step 2: EC2 Linux Setup

- Launch an Ubuntu instance in your favourite region (eg. region `us-east-1`).
- SSH into the instance from your local machine.

### Step 3: Install AWS CLI v2

```shell
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
sudo apt install unzip
unzip awscliv2.zip
sudo ./aws/install -i /usr/local/aws-cli -b /usr/local/bin --update
```

```
aws configure

```

-- Give Required Info in Prompt

```
aws --version
```

# Install AWS CLI v2 on a local machine running macOS.

```bash

curl "https://awscli.amazonaws.com/AWSCLIV2.pkg" -o "AWSCLIV2.pkg"
sudo installer -pkg AWSCLIV2.pkg -target /

```

```
aws --version
```

```
aws configure

```

```
which aws

```

-- Give Required Info in Prompt
