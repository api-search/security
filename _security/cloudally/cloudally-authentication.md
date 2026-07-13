---
api_key_in: []
api_specs:
- filename: cloudally-openapi.yml
  format: yaml
  label: CloudAlly API
  slug: cloudally-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudally/refs/heads/main/openapi/cloudally-openapi.yml
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
- Microsoft 365
- OpenText
- SaaS Backup
- Salesforce
---
