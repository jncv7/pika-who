# pika-who
pika-who is a script that I created for a job that I was working that required me to gather information of an AWS Account's IAM Posture.
It basically is an AWS IAM User Policy Auditing script. It helps with data gathering, and gives you a way to quickly extract the information you need.
This automates the process of auditing AWS IAM users and their associated policies. It retrieves user details, managed and inline policies, analyzes permissions, and generates a detailed Excel report. 
This tool is ideal for security audits, compliance checks, and identifying users with excessive or risky permissions.
I am a pretty beginner coder, but I do enjoy making thing just like this.

### Features

- **IAM User Retrieval**:
  - Fetches all IAM users from AWS with support for pagination.
  
- **Policy Analysis**:
  - Retrieves managed and inline policies for each user.
  - Extracts detailed policy content, including default versions of managed policies.
  - Identifies S3 and IAM-related actions in policy documents for focused analysis.

- **Report Generation**:
  - Outputs an Excel file with the following sheets:
    - **User Summary**: Lists all users and their associated policies.
    - **Managed Policies**: Details managed policies, including ARNs and policy content.
    - **Inline Policies**: Details inline policies and their content.
    - **S3 and IAM Permissions**: Highlights permissions specific to AWS S3 and IAM actions.

- **User Feedback**:
  - Displays Start time and End time in terminal with color-coded messages to support IPE gathering.
  - Includes timestamps for audit tracking.

### Requirements

- Python 3.8+
- AWS credentials with sufficient permissions to access IAM data.
- The following Python libraries:
  - `boto3`
  - `openpyxl`
  - `colorama`

Install the dependencies using `pip`:

```bash
pip install boto3 openpyxl colorama
```

## How can I use it?
- You can copy paste this script into your own file OR download the file. I hope this script helps less tech sauvy people.

