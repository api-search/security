---
api_key_in:
- header
api_specs:
- filename: commvault-rest-openapi.yml
  format: yaml
  label: Commvault REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commvault/refs/heads/main/openapi/commvault-rest-openapi.yml
- filename: commvault-command-center-openapi.yml
  format: yaml
  label: Commvault Command Center API
  slug: command-center-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commvault/refs/heads/main/openapi/commvault-command-center-openapi.yml
- filename: commvault-automation-openapi.yml
  format: yaml
  label: Commvault Automation API
  slug: automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commvault/refs/heads/main/openapi/commvault-automation-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Commvault Authentication
name_suffix: Authentication
oauth_flows: []
overview: Commvault secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Commvault
provider_slug: commvault
scheme_count: 1
schemes:
- description: QSDK authentication token obtained from the Login endpoint.
  in: header
  name: authToken
  parameter: Authtoken
  sources:
  - openapi/commvault-automation-openapi.yml
  - openapi/commvault-command-center-openapi.yml
  - openapi/commvault-rest-openapi.yml
  type: apiKey
slug: commvault-authentication
source_filename: commvault-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/commvault-automation-openapi.yml, openapi/commvault-command-center-openapi.yml,\n  openapi/commvault-rest-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: authToken\n  type: apiKey\n  in: header\n  parameter: Authtoken\n  description: QSDK authentication token obtained from the Login endpoint.\n  sources:\n  - openapi/commvault-automation-openapi.yml\n  - openapi/commvault-command-center-openapi.yml\n  - openapi/commvault-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commvault/refs/heads/main/authentication/commvault-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Backup
- Cloud Storage
- Cyber Recovery
- Data Management
- Data Protection
- Disaster Recovery
- Enterprise Software
---
