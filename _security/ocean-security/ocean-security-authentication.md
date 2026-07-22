---
api_key_in:
- header
api_specs:
- filename: ocean-security-openapi.yml
  format: yaml
  label: Ocean Security API
  slug: ocean-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-security/refs/heads/main/openapi/ocean-security-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ocean Security Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ocean Security secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ocean Security
provider_slug: ocean-security
scheme_count: 1
schemes:
- description: API key for authentication
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/ocean-security-openapi.yml
  type: apiKey
slug: ocean-security-authentication
source_filename: ocean-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/ocean-security-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: API key for authentication\n  sources:\n  - openapi/ocean-security-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ocean-security/refs/heads/main/authentication/ocean-security-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Security
- Email Security
- Cybersecurity
- Phishing
- Threat Detection
- Email
- Anti-Phishing
- Artificial Intelligence
- Threat Intelligence
---
