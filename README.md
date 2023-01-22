# Cloud

Startup infrastructure, scripted.

## Background

I began another project with the intent of deploying it on AWS, then thought better of it. The code will be repurposed simply for research and fun.

## Intent

Exercise precise control over an AWS VPC through targeted information gathering, infrastructure creation and modification scaleable architecture.

The control for the experiment will be a the successful delivery of a boilerplate web application.

Other concerns, such as version management and sophisticated build pipelines are out of scope (for V1 at least).

Major AWS services will include but are not limited to:
- EC2
- ELB
- RDS
- ECR
- Route 53
- S3
- Cloudwatch

Relevant features will include but are not limited to:
- Service scaleability
- Multi-region
- VPC peering
- VPN access
- Data and security compliance

## Status

This projected is the result of gutting another. It's command center was a quite deeply inbedded sub-makefile that received key information from its parent.

In other words, this project doesn't currently work.

Moreover, its structure doesn't indicate that it's quite ready for the task described. It will need to undergo significant refactoring to acheive its useability goals.

## Structure

```
.
├── conf
├── logs
├── Makefile
├── Make.sh
├── README.md
├── resource-type-lists
├── templater.py
└── userdata.sh

3 directories, 5 files
```

<!-- ## AWS Configuration

When running ops from the root Makefile, specify `PERM_MODEL=env` if you're not the author of this project. This will prompt AWS to search first in your environmental vars, then your AWS config file, for necessary parameters such as access key, region, output format, etcetera.

You can also set `env` as default. Change the default parameter in the root Makefile. Change this line: `PERM_MODEL='custom'` to this: `PERM_MODEL='env'`. -->
