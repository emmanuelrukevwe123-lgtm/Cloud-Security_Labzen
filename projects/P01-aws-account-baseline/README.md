# P1 · Secure AWS account baseline

**Goal:** set up the AWS account the way a security team would want it before any workload exists.

| Control | Why | Status |
| --- | --- | --- |
| Account audit (find what already exists) | You can't secure what you don't know about (NIST CSF: Identify) | ✅ 26 Oct: found a running PrestaShop stack ([Project 00](../00-prestashop-on-aws/)) |
| Root user MFA, no root access keys | Root can do anything and can't be restricted | ☐ |
| Zero-spend + $5 budgets, Free Tier alerts | Cost spikes are also a sign of compromise | ☐ |
| IAM Identity Center admin user with MFA | Named, short-lived access instead of root or long-term keys | ☐ |
| AWS CLI via SSO on Kali | No long-term keys on my laptop | ☐ |
| CloudTrail trail (all regions, log validation) | Every API action recorded | ☐ |
| IAM Access Analyzer | Finds resources shared outside the account | ☐ |
| Least-privilege S3 read-only role | Practising least privilege | ☐ |
| Root sign-in alert (EventBridge → SNS) | Know immediately when root is used | ☐ |

_Write-up, screenshots and lessons follow as each control is completed._
