# Benchmark Compliance

This file exaplains which items in the following compliance standards this module covers.

- [CIS Amazon web Services Foundations v1.2.0]
- [AWS Foundational Security Best Practices v1.0.0]

## Definition

Implementation status for each item is categorized as follows.

| Status | Description |
| ------ | ----------- |
| OK | This module ensure that the requirements for this item are satisfied. |
| PARTIAL | This module helps to meet the requirements for this item, but additional work would also be needed. |
| N/A | This module has nothing to do with the requirements for this item. |

## CIS Amazon Web Services Foundations v1.2.0

| No. | Item | Status | Notes |
| ---:| ---- | ------ | ----- |
| 1.1  | Avoid the use of the "root" account | N/A | |
| 1.2  | Ensure multi-factor authentication (MFA) is enabled for all IAM users that have a console password | PARTIAL | Monitored by the AWS Config rule. |
| 1.3  | Ensure credentials unused for 90 days or greater are disabled | PARTIAL | Monitored by the AWS Config rule. |
| 1.4  | Ensure access keys are rotated every 90 days or less | N/A | |
| 1.5  | Ensure IAM password policy requires at least one uppercase letter | OK | |
| 1.6  | Ensure IAM password policy require at least one lowercase letter | OK | |
| 1.7  | Ensure IAM password policy require at least one symbol | OK | |
| 1.8  | Ensure IAM password policy require at least one number | OK | |
| 1.9  | Ensure IAM password policy requires minimum length of 14 or greater | OK | |
| 1.10 | Ensure IAM password policy prevents password reuse | OK | |
| 1.11 | Ensure IAM password policy expires passwords within 90 days or less | OK | |
| 1.12 | Ensure no root account access key exists | N/A | |
| 1.13 | Ensure MFA is enabled for the "root" account | N/A | |
| 1.14 | Ensure hardware MFA is enabled for the "root" account | N/A | |
| 1.15 | Ensure security questions are registered in the AWS account | N/A | |
| 1.16 | Ensure IAM policies are attached only to groups or roles | N/A | |
| 1.17 | Maintain current contact details | N/A | |
| 1.18 | Ensure security contact information is registered | N/A | |
| 1.19 | Ensure IAM instance roles are used for AWS resource access from instances | N/A | |
| 1.20 | Ensure a support role has been created to manage incidents with AWS Support | OK | |
| 1.21 | Do not setup access keys during initial user setup for all IAM users that have a console password | N/A | |
| 1.22 | Ensure IAM policies that allow full "\*:\*" administrative privileges are not created | N/A | |
| 2.1  | Ensure CloudTrail is enabled in all regions | OK | |
| 2.2  | Ensure CloudTrail log file validation is enabled | OK | |
| 2.3  | Ensure the S3 bucket used to store CloudTrail logs is not publicly accessible | OK | |
| 2.4  | Ensure CloudTrail trails are integrated with CloudWatch Logs | OK | |
| 2.5  | Ensure AWS Config is enabled in all regions | OK | |
| 2.6  | Ensure S3 bucket access logging is enabled on the CloudTrail S3 bucket | OK | |
| 2.7  | Ensure CloudTrail logs are encrypted at rest using KMS CMKs | OK | |
| 2.8  | Ensure rotation for customer created CMKs is enabled | OK | |
| 2.9  | Ensure VPC flow logging is enabled in all VPCs | OK | |
| 3.1  | Ensure a log metric filter and alarm exist for unauthorized API calls | OK | |
| 3.2  | Ensure a log metric filter and alarm exist for Management Console sign-in without MFA | OK | |
| 3.3  | Ensure a log metric filter and alarm exist for usage of "root" account | OK | |
| 3.4  | Ensure a log metric filter and alarm exist for IAM policy changes | OK | |
| 3.5  | Ensure a log metric filter and alarm exist for CloudTrail configuration changes | OK | |
| 3.6  | Ensure a log metric filter and alarm exist for AWS Management Console authentication failures | OK | |
| 3.7  | Ensure a log metric filter and alarm exist for disabling or scheduled deletion of customer created CMKs | OK | |
| 3.8  | Ensure a log metric filter and alarm exist for S3 bucket policy changes | OK | |
| 3.9  | Ensure a log metric filter and alarm exist for AWS Config configuration changes | OK | |
| 3.10 | Ensure a log metric filter and alarm exist for security group changes | OK | |
| 3.11 | Ensure a log metric filter and alarm exist for changes to Network Access Control Lists (NACL) | OK | |
| 3.12 | Ensure a log metric filter and alarm exist for changes to network gateways | OK | |
| 3.13 | Ensure a log metric filter and alarm exist for route table changes | OK | |
| 3.14 | Ensure a log metric filter and alarm exist for VPC changes | OK | |
| 4.1  | Ensure no security groups allow ingress from 0.0.0.0/0 to port 22 | N/A | |
| 4.2  | Ensure no security groups allow ingress from 0.0.0.0/0 to port 3389 | N/A | |
| 4.3  | Ensure the default security group of every VPC restricts all traffic | OK | |
| 4.4  | Ensure routing tables for VPC peering are "least access" | N/A | |

## AWS Foundational Security Best Practices v1.0.0

| No. | Item | Status | Notes |
| ---:| ---- | ------ | ----- |
| ACM.1 | Imported ACM certificates should be renewed after a specified time period | N/A | |
| AutoScaling.1 | Auto Scaling groups associated with a load balancer should use load balancer health checks | N/A | |
| CloudTrail.1 | CloudTrail should be enabled and configured with at least one multi-Region trail | OK | |
| CloudTrail.2 | CloudTrail should have encryption at-rest enabled | OK | |
| CodeBuild.1 | CodeBuild GitHub or Bitbucket source repository URLs should use OAuth | N/A | |
| CodeBuild.2 | CodeBuild project environment variables should not contain clear text credentials | N/A | |
| Config.1 | AWS Config should be enabled | OK | |
| DMS.1 | Database Migration Service replication instances should not be public | N/A | |
| EC2.1 | Amazon EBS snapshots should not be public, determined by the ability to be restorable by anyone | N/A | |
| EC2.2 | The VPC default security group should not allow inbound and outbound traffic | N/A | |
| EC2.3 | Attached EBS volumes should be encrypted at-rest | N/A | |
| EC2.4 | Stopped EC2 instances should be removed after a specified time period | N/A | |
| EC2.6 | VPC flow logging should be enabled in all VPCs | N/A | |
| EC2.7 | EBS default encryption should be enabled | N/A | |
| EC2.8 | EC2 instances should use IMDSv2 | N/A | |
| EFS.1 | Amazon EFS should be configured to encrypt file data at-rest using AWS KMS | N/A | |
| ELBv2.1 | Application Load Balancer should be configured to redirect all HTTP requests to HTTPS | N/A | |
| EMR.1 | Amazon EMR cluster master nodes should not have public IP addresses | N/A | |
| ES.1 | Elasticsearch domains should have encryption at-rest enabled | N/A | |
| GuardDuty.1 | GuardDuty should be enabled | OK | |
| IAM.1 | IAM policies should not allow full "*" administrative privileges | N/A | |
| IAM.2 | IAM users should not have IAM policies attached | N/A | |
| IAM.3 | IAM users' access keys should be rotated every 90 days or less | N/A | |
| IAM.4 | IAM root user access key should not exist | N/A | |
| IAM.5 | MFA should be enabled for all IAM users that have a console password | N/A | |
| IAM.6 | Hardware MFA should be enabled for the root user | N/A | |
| IAM.7 | Password policies for IAM users should have strong configurations | OK | |
| IAM.8 | Unused IAM user credentials should be removed | N/A | |
| KMS.1 | IAM customer managed policies should not allow decryption actions on all KMS keys | N/A | |
| KMS.2 | IAM principals should not have IAM inline policies that allow decryption actions on all KMS keys | N/A | |
| Lambda.1 | Lambda functions should prohibit public access by other accounts | N/A | |
| Lambda.2 | Lambda functions should use latest runtimes | N/A | |
| RDS.1 | RDS snapshots should be private | N/A | |
| RDS.2 | RDS DB instances should prohibit public access, determined by the PubliclyAccessible configuration | N/A | |
| RDS.3 | RDS DB instances should have encryption at-rest enabled | N/A | |
| RDS.4 | RDS cluster snapshots and database snapshots should be encrypted at rest | N/A | |
| RDS.5 | RDS DB instances should be configured with multiple Availability Zones | N/A | |
| RDS.6 | Enhanced monitoring should be configured for RDS DB instances and clusters | N/A | |
| RDS.7 | RDS clusters should have deletion protection enabled | N/A | |
| RDS.8 | RDS DB instances should have deletion protection enabled | N/A | |
| S3.1 | S3 Block Public Access setting should be enabled | PARTIAL | All S3 buckets created by this module block public access. |
| S3.2 | S3 buckets should prohibit public read access | PARTIAL | All S3 buckets created by this module block public read access. |
| S3.3 | S3 buckets should prohibit public write access | PARTIAL | All S3 buckets created by this module block public write access. |
| S3.4 | S3 buckets should have server-side encryption enabled | PARTIAL | All S3 buckets created by this module enable server-side encryption. |
| S3.5 | S3 buckets should require requests to use Secure Socket Layer | PARTIAL | All S3 buckets created by this module block non-SSL requests. |
| S3.6 | Amazon S3 permissions granted to other AWS accounts in bucket policies should be restricted | N/A | |
| SageMaker.1 | SageMaker notebook instances should not have direct internet access | N/A | |
| SecretsManager.1 | Secrets Manager secrets should have automatic rotation enabled | N/A | |
| SecretsManager.2 | Secrets Manager secrets configured with automatic rotation should rotate successfully | N/A | |
| SSM.1 | EC2 instances should be managed by AWS Systems Manager | N/A | |
| SSM.2 | All EC2 instances managed by Systems Manager should be compliant with patching requirements | N/A | |
| SSM.3 | Instances managed by Systems Manager should have an association compliance status of COMPLIANT | N/A | |

[CIS Amazon Web Services Foundations v1.2.0]: https://www.cisecurity.org/benchmark/amazon_web_services/
[AWS Foundational Security Best Practices v1.0.0]: https://docs.aws.amazon.com/securityhub/latest/userguide/securityhub-standards-fsbp.html
