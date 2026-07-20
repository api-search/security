---
api_key_in: []
api_specs:
- filename: eon-openapi-original.yml
  format: yaml
  label: Eon API
  slug: eon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-openapi-original.yml
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
