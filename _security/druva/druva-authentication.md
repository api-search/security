---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Druva Authentication
name_suffix: Authentication
oauth_flows: []
overview: Druva secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Druva
provider_slug: druva
scheme_count: 1
schemes:
- description: Bearer access token obtained from /token using API credentials
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/druva-openapi.yml
  type: http
slug: druva-authentication
source_filename: druva-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/druva-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer access token obtained from /token using API credentials\n  sources:\n  - openapi/druva-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/authentication/druva-authentication.yml
summary_line: http · 1 scheme
tags:
- Backup
- Cyber Resilience
- Data Protection
- Disaster Recovery
- SaaS Backup
---
