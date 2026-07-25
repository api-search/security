---
api_key_in: []
api_specs:
- filename: eon-accounts-api-openapi.yml
  format: yaml
  label: Eon accounts API
  slug: eon-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-accounts-api-openapi.yml
- filename: eon-actionapprovals-api-openapi.yml
  format: yaml
  label: Eon actionApprovals API
  slug: eon-actionapprovals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-actionapprovals-api-openapi.yml
- filename: eon-auth-api-openapi.yml
  format: yaml
  label: Eon auth API
  slug: eon-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-auth-api-openapi.yml
- filename: eon-backuppolicies-api-openapi.yml
  format: yaml
  label: Eon backupPolicies API
  slug: eon-backuppolicies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-backuppolicies-api-openapi.yml
- filename: eon-backups-api-openapi.yml
  format: yaml
  label: Eon backups API
  slug: eon-backups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-backups-api-openapi.yml
- filename: eon-billing-api-openapi.yml
  format: yaml
  label: Eon billing API
  slug: eon-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-billing-api-openapi.yml
- filename: eon-dashboard-api-openapi.yml
  format: yaml
  label: Eon dashboard API
  slug: eon-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-dashboard-api-openapi.yml
- filename: eon-databasesnapshots-api-openapi.yml
  format: yaml
  label: Eon databaseSnapshots API
  slug: eon-databasesnapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-databasesnapshots-api-openapi.yml
- filename: eon-iam-api-openapi.yml
  format: yaml
  label: Eon iam API
  slug: eon-iam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-iam-api-openapi.yml
- filename: eon-jobs-api-openapi.yml
  format: yaml
  label: Eon jobs API
  slug: eon-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-jobs-api-openapi.yml
- filename: eon-resources-api-openapi.yml
  format: yaml
  label: Eon resources API
  slug: eon-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-resources-api-openapi.yml
- filename: eon-snapshots-api-openapi.yml
  format: yaml
  label: Eon snapshots API
  slug: eon-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-snapshots-api-openapi.yml
- filename: eon-vaults-api-openapi.yml
  format: yaml
  label: Eon vaults API
  slug: eon-vaults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-vaults-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
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
