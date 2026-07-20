---
api_key_in: []
api_specs:
- filename: automat-extract-openapi.json
  format: json
  label: Automat Extract API
  slug: automat-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automat/refs/heads/main/openapi/automat-extract-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Automat Authentication
name_suffix: Authentication
oauth_flows: []
overview: Automat secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Automat
provider_slug: automat
scheme_count: 1
schemes:
- name: BearerAuthScheme
  scheme: bearer
  sources:
  - openapi/automat-extract-openapi.json
  type: http
slug: automat-authentication
source_filename: automat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/automat-extract-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuthScheme\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/automat-extract-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/automat/refs/heads/main/authentication/automat-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Enterprise Saas
- Automation
- RPA
- Robotic Process Automation
- Document Extraction
- IDP
- iPaaS
- AI Agents
- Computer Use
- Document Processing
---
