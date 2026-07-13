---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Rightsline Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rightsline secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rightsline
provider_slug: rightsline
scheme_count: 1
schemes:
- description: Bearer token obtained by exchanging Company API Key + Access Key + Secret Access Key. Generate credentials in app.rightsline.com Profile > API Access.
  in: header
  name: ApiKey
  parameter: Authorization
  sources:
  - openapi/rightsline-openapi.yml
  type: apiKey
slug: rightsline-authentication
source_filename: rightsline-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rightsline-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Bearer token obtained by exchanging Company API Key + Access Key + Secret Access\n    Key. Generate credentials in app.rightsline.com Profile > API Access.\n  sources:\n  - openapi/rightsline-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rightsline/refs/heads/main/authentication/rightsline-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Content Management
- Entertainment
- Media
- Rights Management
- Royalties
---
