---
api_key_in:
- header
api_specs:
- filename: seon-docs-openapi.yml
  format: yaml
  label: SEON Fraud API
  slug: fraud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seon-docs/refs/heads/main/openapi/seon-docs-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Seon Docs Authentication
name_suffix: Authentication
oauth_flows: []
overview: SEON secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SEON
provider_slug: seon-docs
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: X-API-KEY
  sources:
  - openapi/seon-docs-openapi.yml
  type: apiKey
slug: seon-docs-authentication
source_filename: seon-docs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/seon-docs-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/seon-docs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seon-docs/refs/heads/main/authentication/seon-docs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AML Compliance
- Fraud Prevention
- Identity Verification
- Risk Scoring
---
