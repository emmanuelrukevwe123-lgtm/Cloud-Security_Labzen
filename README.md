# Cloud Security Labs

Hands-on AWS (and later Azure) projects on my way to **cloud security**, built in public and documented as I learn. Each project covers what I built, the security decisions, how I tested it, how I'd detect an attack on it, and what it cost.

**Goal:** job-ready in cloud security by April 2027, without dropping blue teaming.
**Primary cloud:** AWS · **Second cloud:** Azure · **Tools:** AWS CLI, Terraform, Wazuh, GitHub Actions

Companion repo (SOC / blue team home lab): [soc-home-lab](https://github.com/emmanuelrukevwe123-lgtm/soc-home-lab)

## Projects

| # | Project | Skills | Status |
| --- | --- | --- | --- |
| 00 | [Deploying PrestaShop on AWS, and what I'd do more securely now](projects/00-prestashop-on-aws/) | EC2, RDS, VPC, security review, cost | ✅ Write-up in progress |
| P1 | [Secure AWS account baseline](projects/P01-aws-account-baseline/) | Root MFA, budgets, IAM Identity Center, CloudTrail, alerts | 🔄 Week 1–2 |
| P3 | Secure static website: S3 + CloudFront + WAF | S3, KMS, OAC, WAF, logging | Planned (Nov–Dec) |
| P6 | Secure serverless API with Cognito login | Lambda, API Gateway, DynamoDB, Cognito, JWT | Planned (Jan) |
| P8 | Hybrid cloud SIEM: CloudTrail → Wazuh | CloudTrail, detection engineering | Planned (Jan) |
| P9 | Cloud posture assessment | Security Hub, Config, Prowler, CIS | Planned (Feb) |
| P10 | Automated threat response | GuardDuty, EventBridge, Lambda (Python) | Planned (Feb) |
| P11 | Cloud incident simulations | Incident response, forensics, reporting | Planned (Mar) |
| P12 | Secure IaC pipeline | Terraform, Checkov, GitHub Actions, OIDC | Planned (Mar) |
| P13 | Multi-cloud SIEM with Microsoft Sentinel | Azure, Entra ID, KQL | Planned (Apr) |
| ★ | Capstone: secure 3-tier app with detection and response | Everything above | Planned (Apr) |

Blue-team projects (network, web, phishing and Windows/AD detection) live in [soc-home-lab](https://github.com/emmanuelrukevwe123-lgtm/soc-home-lab).

## Repo layout

| Path | Contents |
| --- | --- |
| `projects/` | One folder per project: write-up (`README.md`) and redacted screenshots |
| `infra/aws/` | Terraform code (from week 7) |
| `notes/` | Glossary, cheat sheets, what I'm learning |
| `progress-log.md` | Session-by-session log |

## Rules I follow

- Budget alerts before building anything; everything torn down after each session.
- No access keys, account IDs, emails or Terraform state in this repo; screenshots are redacted.
- Only my own accounts and resources are ever tested.

## License

[MIT](LICENSE) © 2026 Emmanuel Nwabuokei
