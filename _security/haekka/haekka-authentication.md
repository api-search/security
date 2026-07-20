---
api_key_in: []
api_specs:
- filename: haekka-public-api-openapi.yml
  format: yaml
  label: Haekka Public API
  slug: haekka-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haekka/refs/heads/main/openapi/haekka-public-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Haekka Authentication
name_suffix: Authentication
oauth_flows: []
overview: Haekka secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Haekka
provider_slug: haekka
scheme_count: 1
schemes:
- description: 'API key generated in Haekka account settings, passed as `Authorization: Bearer {key}`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/haekka-public-api-openapi.yml
  type: http
slug: haekka-authentication
source_filename: haekka-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/haekka-public-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key generated in Haekka account settings, passed as `Authorization: Bearer\n    {key}`.'\n  sources:\n  - openapi/haekka-public-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/haekka/refs/heads/main/authentication/haekka-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security Awareness Training
- Compliance Training
- Microlearning
- Slack
- Phishing Simulation
- Employee Training
- HIPAA
- SOC 2
- API
---
