---
api_key_in:
- header
api_specs:
- filename: ironcore-labs-vendor-bridge-openapi.yml
  format: yaml
  label: IronCore Vendor API Bridge
  slug: ironcore-vendor-api-bridge
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironcore-labs/refs/heads/main/openapi/ironcore-labs-vendor-bridge-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ironcore Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: IronCore Labs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: IronCore Labs
provider_slug: ironcore-labs
scheme_count: 1
schemes:
- description: 'VAB authorization header. Form: `vab:1:<API_KEY>`'
  in: header
  name: Authorization
  parameter: Authorization
  sources:
  - openapi/ironcore-labs-vendor-bridge-openapi.yml
  type: apiKey
slug: ironcore-labs-authentication
source_filename: ironcore-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/ironcore-labs-vendor-bridge-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Authorization\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'VAB authorization header. Form: `vab:1:<API_KEY>`'\n  sources:\n  - openapi/ironcore-labs-vendor-bridge-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ironcore-labs/refs/heads/main/authentication/ironcore-labs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Encryption
- Data Privacy
- Security
- Application-Layer Encryption
- Key Management
- Cryptography
- AI
- Vector Database
- SaaS
---
