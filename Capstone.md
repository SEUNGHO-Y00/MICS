# CYBER 295 Capstone

## My Privacy Switch Consent Management Platform on AWS

## Overview

This project provisions the **Consumer Privacy driven Consent Management Platform (CMP)** infrastructure on AWS using **Terraform**. The architecture follows a **microservices** approach with **ECS Fargate**, **API Gateway**, **DynamoDB**, and other AWS services to handle user consent management in a secure, scalable, and compliant way.

## Project Structure

```
T2.3_infra/
├── env
│   ├── dev
│   └── ──modules
│   │   └── s3/
│   │   │    ├── main.tf
│   │   │    ├── outputs.tf
│   │   │    ├── variables.tf
│   │   └── ec2/
│   │   ├── main.tf
│   │   ├── outputs.tf
│   │   ├── variables.tf
│   │   └── s3/
│   │   ├── main.tf
│   │   ├── outputs.tf
│   │   ├── variables.tf
│   │   └── rds/
│   │   ├── main.tf
│   │   ├── outputs.tf
│   │   ├── variables.tf
│
```

- **`modules/`**: Contains reusable Terraform modules for provisioning DynamoDB, API Gateway, IAM roles, and other resources.
- **`environments/`**: Holds environment-specific Terraform configurations for `dev`, `prod`, etc.
- **`global/`**: Defines global variables and provider configurations shared across environments.

## Requirements

- Terraform >= 0.12.x
- AWS CLI configured with appropriate credentials
- AWS IAM permissions to provision resources like VPC, ECS, DynamoDB, API Gateway, and IAM roles.

## How to Use

### 1. Clone the repository

```bash
git clone https://github.com/your-repo/terraform-consent-management.git
cd terraform-consent-management
```

## myps

### Create Directories for the following:
 - psconsent - consent modal cookie banner
 - psportal - Central PrivacySwitch.org user consent prefrences and tracking
 - pstoolbar - toolbar UX
 - participatingsite1 - html / css / js and assets for site 1 - PowerTools
 - participatingsite2 - html / css / js and assets for site 2 - EliteRides
 - participatingsite3 - html / css / js and assets for site 3 - ForeverFlowers
 - pscurrency - blockchain

### Database
- User Table
- User 1:
   - Global Default Prefences - Purpose to populate defaults for each site user visits
      - Functional: True / False
      - Analytical: True / False
      - Marketing: True / False

    Allows us to populate defaults on each new site that the user is visiting for the first time.
    writePref(userID)
    readPrefs(userID)

    - Site Level Preferences - Record consents for each site user visits
       - Site 1
          - Functional: T/F
          - A: T/F
          - M: T/F
       - Site 2
         - F: T/F
         - A: T/F
         - M: T/F
     Allows us to create the protal page for each user.

     API:
      writePrefs (userID, SiteID, Preferences)
      readPrefs (userID, SiteID) -> return empty if none

- User 2

### Sites
 - participatingsite1 - html / css / js and assets for site 1 - PowerTools
   - Create subdomain - Dele
   - Get HTTPS certs
   - Load up HTML - Aravind
 - participatingsite2 - html / css / js and assets for site 2 - EliteRides
   - Create subdomain - Dele
   - Get HTTPS certs
   - Reformat Site Template
 - participatingsite3 - html / css / js and assets for site 3 - ForeverFlowers

