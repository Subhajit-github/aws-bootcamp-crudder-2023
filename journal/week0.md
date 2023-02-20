# Week 0 — Billing and Architecture

## Getting the AWS CLI Working

Installed AWS CLI and configured it with my IAM User Credentials.

Updated my `.gitpod.yml` to include the following task.

```sh
tasks:
  - name: aws-cli
    env:
      AWS_CLI_AUTO_PROMPT: on-partial
    init: |
      cd /workspace
      curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
      unzip awscliv2.zip
      sudo ./aws/install
      cd $THEIA_WORKSPACE_ROOT
```

### Create a new User and Generate AWS Credentials


![Installing AWS CLI and configure user](assets/user-proof.jpg)

### Add a billing alarm

Added cloudwatch billing alarm
![Image of the alarm I created](assets/Billing Alarm.jpg)

### Add a budget

Added cloudwatch billing alarm
![Image of the alarm I created](assets/Budget.jpg)

### Lucidchart Napkin Diagram

Created Lucid Chart Napkin Diagram

![Image of Napkin Diagram](assets/Napkin%20Diagram.jpg)

![Napkin Diagram view link](https://lucid.app/lucidchart/fef713ef-1011-4771-a337-a29b172c599b/edit?viewport_loc=-10%2C-58%2C1707%2C811%2C0_0&invitationId=inv_f05c0fa2-be45-4f38-a306-cbc7aa1422bf)

### Logical Architecture Diagram

Created Lucid Chart Architectural Diagram

![Image of Architectural Diagram](assets/Logical%20Architecture.jpg)

![Logical Architecture Diagram link](https://lucid.app/lucidchart/466802df-b4c0-4fa0-b66b-7803ccdbf67a/edit?viewport_loc=-55%2C43%2C1929%2C916%2C0_0&invitationId=inv_d57b3f11-00b4-4847-b072-e1909117a04a)
