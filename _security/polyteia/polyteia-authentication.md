---
api_key_in: []
api_specs:
- filename: polyteia-platform-openapi.yml
  format: yaml
  label: Polyteia Platform API
  slug: polyteia-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polyteia/refs/heads/main/openapi/polyteia-platform-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Polyteia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Polyteia secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Polyteia
provider_slug: polyteia
scheme_count: 1
schemes:
- bearerFormat: PAK
  description: 'Personal Access Key (PAK). A PAK impersonates the issuing account and carries that account''s permissions. Presented as `Authorization: Bearer <PAK>`.'
  name: PersonalAccessKey
  scheme: bearer
  sources:
  - openapi/polyteia-platform-openapi.yml
  type: http
slug: polyteia-authentication
source_filename: polyteia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/polyteia-platform-openapi.yml\ndocs: https://docs.polyteia.com/api-docs/en/authentication.md\nnotes: >\n  Polyteia authenticates API requests with a Personal Access Key (PAK) presented\n  as an HTTP Bearer token (`Authorization: Bearer <PAK>`). A PAK impersonates the\n  issuing account and inherits that account's permissions; there is no separate\n  OAuth scope surface. PAKs are created from Account > Security & Access in the\n  platform UI and are shown only once at creation.\nsummary:\n  types:\n  - http\nschemes:\n- name: PersonalAccessKey\n  type: http\n  scheme: bearer\n  bearerFormat: PAK\n  description: 'Personal Access Key (PAK). A PAK impersonates the issuing account and carries\n    that account''s permissions. Presented as `Authorization: Bearer <PAK>`.'\n  sources:\n  - openapi/polyteia-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polyteia/refs/heads/main/authentication/polyteia-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai Enterprise Software
- GovTech
- Public Sector
- Data Platform
- Government
- Data Analytics
- Germany
- Business Intelligence
- No-Code
---
