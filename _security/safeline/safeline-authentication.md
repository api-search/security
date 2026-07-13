---
api_key_in:
- header
api_specs:
- filename: safeline-management-openapi.yml
  format: yaml
  label: SafeLine Management API
  slug: safeline
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/safeline/refs/heads/main/openapi/safeline-management-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Safeline Authentication
name_suffix: Authentication
oauth_flows: []
overview: SafeLine secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SafeLine
provider_slug: safeline
scheme_count: 1
schemes:
- description: API token obtained from the SafeLine management interface
  in: header
  name: APITokenAuth
  parameter: X-SLCE-API-Token
  sources:
  - openapi/safeline-management-openapi.yml
  type: apiKey
slug: safeline-authentication
source_filename: safeline-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/safeline-management-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APITokenAuth\n  type: apiKey\n  in: header\n  parameter: X-SLCE-API-Token\n  description: API token obtained from the SafeLine management interface\n  sources:\n  - openapi/safeline-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/safeline/refs/heads/main/authentication/safeline-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Proxy
- WAF
- Security
- Open Source
- Reverse Proxy
- API Gateway
---
