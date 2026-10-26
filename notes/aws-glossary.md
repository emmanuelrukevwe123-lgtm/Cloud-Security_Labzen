# AWS glossary

| Term | Meaning | Home-lab twin |
| --- | --- | --- |
| **AWS** | Amazon's cloud: computers, storage and networks rented by the hour | My laptop running VMs |
| **Region** (e.g. eu-west-2 London, eu-north-1 Stockholm) | A geographic area with AWS data centres | |
| **Availability zone** (e.g. eu-north-1b) | One or more separate data centres inside a region; using several survives a failure | |
| **EC2** (Elastic Compute Cloud) | Virtual machines, called instances | My Ubuntu VM |
| **Instance type** (e.g. t3.micro) | The VM size: family (t3 = cheap, general purpose) + size (micro = 2 vCPUs, 1 GB RAM) | VM CPU/RAM settings |
| **AMI** (Amazon Machine Image) | A template/backup of a server's disk that new instances start from | A VM snapshot/template |
| **EBS** (Elastic Block Store) | The network disk attached to an instance | A virtual disk |
| **RDS** (Relational Database Service) | A managed database: AWS runs and patches the server, I configure and use it | A MySQL VM I'd maintain myself |
| **db.t4g.micro** | A database size ("g" = AWS Graviton ARM processor) | |
| **Aurora** | AWS's own high-performance MySQL/PostgreSQL-compatible database | |
| **VPC** (Virtual Private Cloud) | My private network in AWS: address range, subnets, routes, firewalls | My pfSense network |
| **Default VPC** (172.31.0.0/16) | A ready-made VPC in every region, public-facing by default: easy, not secure by design | |
| **Subnet** | A slice of the VPC in one availability zone; public if its route table points to an internet gateway | A pfSense zone |
| **Security group** | A stateful firewall attached to an instance or database | pfSense rules |
| **S3** (Simple Storage Service) | Object storage in "buckets": backups, images, logs, websites | A file share |
| **Lambda** | Serverless functions that run only when triggered | |
| **CloudWatch** | Metrics, logs and alarms | Part of Wazuh |
| **CloudTrail** | The audit log of every API call in the account | Wazuh's audit trail |
| **IAM** | Identity and Access Management: users, roles, policies | Linux users and permissions |
| **ARN** (Amazon Resource Name) | A unique ID for any resource, used in IAM policies | |
| **Credits** | Free AWS money on the free plan, used up by running resources | |
| **Amazon Q** | AWS's AI assistant in the console | |
| **CloudShell** | A browser terminal with the AWS CLI already signed in | A terminal on Kali |
| **LAMP stack** | Linux + Apache + MySQL + PHP: the classic web app setup | |
