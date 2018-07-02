# amazon-guardduty-ec2-threat-detection

Illustrate the capabilities of Amazon GuardDuty to detect EC2 threats

![Final Environment](https://user-images.githubusercontent.com/3911650/42183996-13a10820-7e01-11e8-906b-1974b24a2eba.png)

## Getting Started

Deploy the CloudFormation `infrastructure/cloudformation.json` template. The template creates a user with the following credentials and minimal required permisisons to complete the Lab:

- Username: _student_
- Password: _password_

## Instructions

1. Enable GuardDuty in the AWS Management Console

1. Save the public IPv4 address of the EC2 instance named __Malicious Instance__ to a plain text file named `threat-list.txt`

1. Upload `threat-list.txt` to the S3 bucket with threatlist in its name

1. In the GuardDuty Console, navigate to __Lists__ and activate a new threat list by using the S3 link to threat-list.txt. Ensure you check __Activate__ to instruct GuardDuty to use the threat list.

1. Periodically refresh the GuardDuty findings table to view the findings related to the Lab environment. It may take up to 10 minutes to view all three.

## Cleaning Up

Delete the CloudFormation stack to remove all the resources used in the Lab.