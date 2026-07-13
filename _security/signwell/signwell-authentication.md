---
api_key_in:
- header
api_specs:
- filename: llms.txt
  format: yaml
  label: SignWell API
  slug: signwell-api
  spec_type: OpenAPI
  url: https://developers.signwell.com/llms.txt
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Signwell Authentication
name_suffix: Authentication
oauth_flows: []
overview: SignWell secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SignWell
provider_slug: signwell
scheme_count: 1
schemes:
- in: header
  name: api_key
  parameter: X-Api-Key
  sources:
  - openapi/signwell-signwell-api-openapi.yml
  type: apiKey
slug: signwell-authentication
source_filename: signwell-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/signwell-signwell-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/signwell-signwell-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/signwell/refs/heads/main/authentication/signwell-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- E-Signature
- Electronic Signature
- Documents
- PDF
- Signing
- Templates
- Workflows
- HIPAA
- SOC2
---
