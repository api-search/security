---
api_key_in: []
api_specs:
- filename: cloudally-authentication-api-openapi.yml
  format: yaml
  label: CloudAlly Authentication API
  slug: cloudally-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudally/refs/heads/main/openapi/cloudally-authentication-api-openapi.yml
- filename: cloudally-backups-api-openapi.yml
  format: yaml
  label: CloudAlly Backups API
  slug: cloudally-backups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudally/refs/heads/main/openapi/cloudally-backups-api-openapi.yml
- filename: cloudally-billing-api-openapi.yml
  format: yaml
  label: CloudAlly Billing API
  slug: cloudally-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudally/refs/heads/main/openapi/cloudally-billing-api-openapi.yml
- filename: cloudally-partners-api-openapi.yml
  format: yaml
  label: CloudAlly Partners API
  slug: cloudally-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudally/refs/heads/main/openapi/cloudally-partners-api-openapi.yml
- filename: cloudally-restore-api-openapi.yml
  format: yaml
  label: CloudAlly Restore API
  slug: cloudally-restore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudally/refs/heads/main/openapi/cloudally-restore-api-openapi.yml
- filename: cloudally-tasks-api-openapi.yml
  format: yaml
  label: CloudAlly Tasks API
  slug: cloudally-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudally/refs/heads/main/openapi/cloudally-tasks-api-openapi.yml
- filename: cloudally-users-api-openapi.yml
  format: yaml
  label: CloudAlly Users API
  slug: cloudally-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudally/refs/heads/main/openapi/cloudally-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cloudally Authentication
name_suffix: Authentication
oauth_flows: []
overview: CloudAlly secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CloudAlly
provider_slug: cloudally
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cloudally-openapi.yml
  type: http
slug: cloudally-authentication
source_filename: cloudally-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloudally-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/cloudally-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudally/refs/heads/main/authentication/cloudally-authentication.yml
summary_line: http · 1 scheme
tags:
- Backup
- Box
- Data Protection
- Disaster Recovery
- Dropbox
- Google Workspace
- Microsoft-365
- OpenText
- SaaS Backup
- Salesforce
---
