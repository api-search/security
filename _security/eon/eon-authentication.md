---
anonymous_access: false
api_key_in: []
api_specs:
- filename: eon-accounts-api-openapi.yml
  format: yaml
  label: Eon Accounts API
  slug: eon-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-accounts-api-openapi.yml
- filename: eon-actionapprovals-api-openapi.yml
  format: yaml
  label: Eon Action Approvals API
  slug: eon-actionapprovals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-actionapprovals-api-openapi.yml
- filename: eon-auth-api-openapi.yml
  format: yaml
  label: Eon Auth API
  slug: eon-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-auth-api-openapi.yml
- filename: eon-backups-api-openapi.yml
  format: yaml
  label: Eon Backups API
  slug: eon-backups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-backups-api-openapi.yml
- filename: eon-billing-api-openapi.yml
  format: yaml
  label: Eon Billing API
  slug: eon-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-billing-api-openapi.yml
- filename: eon-dashboard-api-openapi.yml
  format: yaml
  label: Eon Dashboard API
  slug: eon-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-dashboard-api-openapi.yml
- filename: eon-iam-api-openapi.yml
  format: yaml
  label: Eon Iam API
  slug: eon-iam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-iam-api-openapi.yml
- filename: eon-jobs-api-openapi.yml
  format: yaml
  label: Eon Jobs API
  slug: eon-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-jobs-api-openapi.yml
- filename: eon-resources-api-openapi.yml
  format: yaml
  label: Eon Resources API
  slug: eon-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-resources-api-openapi.yml
- filename: eon-snapshots-api-openapi.yml
  format: yaml
  label: Eon Snapshots API
  slug: eon-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-snapshots-api-openapi.yml
- filename: eon-vaults-api-openapi.yml
  format: yaml
  label: Eon Vaults API
  slug: eon-vaults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-vaults-api-openapi.yml
- filename: eon-backup-policies-api-openapi.yml
  format: yaml
  label: Eon Backup Policies API
  slug: eon-backup-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-backup-policies-api-openapi.yml
- filename: eon-database-snapshots-api-openapi.yml
  format: yaml
  label: Eon Database Snapshots API
  slug: eon-database-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-database-snapshots-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Eon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eon secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Eon
provider_slug: eon
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/eon-openapi-original.yml
  type: http
slug: eon-authentication
source_filename: eon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/eon-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/eon-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/authentication/eon-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Cloud Backup
- Data Protection
- Disaster Recovery
- Ransomware Protection
- Backup
- Cloud Storage
- Data Lake
- Multi-Cloud
- Azure
- Google Cloud
---
