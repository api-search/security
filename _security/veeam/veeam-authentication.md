---
api_key_in:
- header
api_specs:
- filename: vspc-rest.html
  format: yaml
  label: Veeam Service Provider Console REST API
  slug: veeam-service-provider-console-rest-api
  spec_type: OpenAPI
  url: https://helpcenter.veeam.com/docs/vac/rest/reference/vspc-rest.html
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Veeam Authentication
name_suffix: Authentication
oauth_flows: []
overview: Veeam secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Veeam
provider_slug: veeam
scheme_count: 1
schemes:
- description: Bearer \<JWT\>
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/veeam-backup-aws-openapi.yml
  - openapi/veeam-backup-replication-openapi.yml
  type: apiKey
slug: veeam-authentication
source_filename: veeam-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/veeam-backup-aws-openapi.yml, openapi/veeam-backup-replication-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Bearer \\<JWT\\>\n  sources:\n  - openapi/veeam-backup-aws-openapi.yml\n  - openapi/veeam-backup-replication-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veeam/refs/heads/main/authentication/veeam-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Backup
- Data Management
- Disaster Recovery
- Cloud Backup
- Restore
- Replication
- Data Protection
- Microsoft 365
- Azure
- Google Cloud
- Ransomware Recovery
---
