---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cloudally-api-authorization-api-openapi.yml
  format: yaml
  label: CloudAlly API Authorization API
  slug: cloudally-api-authorization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudally/openapi/cloudally-api-authorization-api-openapi.yml
- filename: cloudally-backup-management-api-openapi.yml
  format: yaml
  label: CloudAlly Backup management API
  slug: cloudally-backup-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudally/openapi/cloudally-backup-management-api-openapi.yml
- filename: cloudally-billing-management-api-openapi.yml
  format: yaml
  label: CloudAlly Billing management API
  slug: cloudally-billing-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudally/openapi/cloudally-billing-management-api-openapi.yml
- filename: cloudally-distributor-backup-management-api-openapi.yml
  format: yaml
  label: CloudAlly Distributor Backup management API
  slug: cloudally-distributor-backup-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudally/openapi/cloudally-distributor-backup-management-api-openapi.yml
- filename: cloudally-partner-portal-api-openapi.yml
  format: yaml
  label: CloudAlly Partner Portal API
  slug: cloudally-partner-portal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudally/openapi/cloudally-partner-portal-api-openapi.yml
- filename: cloudally-reseller-backup-management-api-openapi.yml
  format: yaml
  label: CloudAlly Reseller Backup management API
  slug: cloudally-reseller-backup-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudally/openapi/cloudally-reseller-backup-management-api-openapi.yml
- filename: cloudally-restore-download-api-openapi.yml
  format: yaml
  label: CloudAlly Restore & Download API
  slug: cloudally-restore-download-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudally/openapi/cloudally-restore-download-api-openapi.yml
- filename: cloudally-user-management-api-openapi.yml
  format: yaml
  label: CloudAlly User management API
  slug: cloudally-user-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudally/openapi/cloudally-user-management-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
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
source_yaml_url: https://artifacts.apis.io/cloudally/authentication/cloudally-authentication.yml
summary_line: http · 1 scheme
tags:
- Backup
- Box
- Data Protection
- Disaster Recovery
- Dropbox
- Google Workspace
- Microsoft 365
- OpenText
- SaaS Backup
- Salesforce
---
