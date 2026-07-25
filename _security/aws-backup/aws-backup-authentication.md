---
api_key_in:
- header
api_specs:
- filename: aws-backup-backup-jobs-api-openapi.yml
  format: yaml
  label: AWS Backup Backup Jobs API
  slug: aws-backup-backup-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-backup/refs/heads/main/openapi/aws-backup-backup-jobs-api-openapi.yml
- filename: aws-backup-backup-plans-api-openapi.yml
  format: yaml
  label: AWS Backup Backup Plans API
  slug: aws-backup-backup-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-backup/refs/heads/main/openapi/aws-backup-backup-plans-api-openapi.yml
- filename: aws-backup-backup-selections-api-openapi.yml
  format: yaml
  label: AWS Backup Backup Selections API
  slug: aws-backup-backup-selections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-backup/refs/heads/main/openapi/aws-backup-backup-selections-api-openapi.yml
- filename: aws-backup-backup-vaults-api-openapi.yml
  format: yaml
  label: AWS Backup Backup Vaults API
  slug: aws-backup-backup-vaults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-backup/refs/heads/main/openapi/aws-backup-backup-vaults-api-openapi.yml
- filename: aws-backup-copy-jobs-api-openapi.yml
  format: yaml
  label: AWS Backup Copy Jobs API
  slug: aws-backup-copy-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-backup/refs/heads/main/openapi/aws-backup-copy-jobs-api-openapi.yml
- filename: aws-backup-frameworks-api-openapi.yml
  format: yaml
  label: AWS Backup Frameworks API
  slug: aws-backup-frameworks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-backup/refs/heads/main/openapi/aws-backup-frameworks-api-openapi.yml
- filename: aws-backup-recovery-points-api-openapi.yml
  format: yaml
  label: AWS Backup Recovery Points API
  slug: aws-backup-recovery-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-backup/refs/heads/main/openapi/aws-backup-recovery-points-api-openapi.yml
- filename: aws-backup-report-plans-api-openapi.yml
  format: yaml
  label: AWS Backup Report Plans API
  slug: aws-backup-report-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-backup/refs/heads/main/openapi/aws-backup-report-plans-api-openapi.yml
- filename: aws-backup-restore-jobs-api-openapi.yml
  format: yaml
  label: AWS Backup Restore Jobs API
  slug: aws-backup-restore-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-backup/refs/heads/main/openapi/aws-backup-restore-jobs-api-openapi.yml
- filename: aws-backup-tags-api-openapi.yml
  format: yaml
  label: AWS Backup Tags API
  slug: aws-backup-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-backup/refs/heads/main/openapi/aws-backup-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Aws Backup Authentication
name_suffix: Authentication
oauth_flows: []
overview: AWS Backup secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AWS Backup
provider_slug: aws-backup
scheme_count: 1
schemes:
- description: AWS Signature Version 4 signed Authorization header
  in: header
  name: SigV4
  parameter: Authorization
  sources:
  - openapi/aws-backup-openapi.yml
  type: apiKey
slug: aws-backup-authentication
source_filename: aws-backup-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aws-backup-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SigV4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 signed Authorization header\n  sources:\n  - openapi/aws-backup-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aws-backup/refs/heads/main/authentication/aws-backup-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Backup
- Data Protection
- Disaster Recovery
- Managed Service
- Compliance
---
