---
api_key_in:
- header
api_specs:
- filename: seon-tech-openapi.yml
  format: yaml
  label: SEON Fraud API
  slug: fraud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seon-tech/refs/heads/main/openapi/seon-tech-openapi.yml
- filename: seon-tech-openapi.yml
  format: yaml
  label: SEON Email API
  slug: email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seon-tech/refs/heads/main/openapi/seon-tech-openapi.yml
- filename: seon-tech-openapi.yml
  format: yaml
  label: SEON Phone API
  slug: phone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seon-tech/refs/heads/main/openapi/seon-tech-openapi.yml
- filename: seon-tech-openapi.yml
  format: yaml
  label: SEON IP API
  slug: ip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seon-tech/refs/heads/main/openapi/seon-tech-openapi.yml
- filename: seon-tech-openapi.yml
  format: yaml
  label: SEON BIN API
  slug: bin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seon-tech/refs/heads/main/openapi/seon-tech-openapi.yml
- filename: seon-tech-openapi.yml
  format: yaml
  label: SEON AML API
  slug: aml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seon-tech/refs/heads/main/openapi/seon-tech-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Seon Tech Authentication
name_suffix: Authentication
oauth_flows: []
overview: SEON secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SEON
provider_slug: seon-tech
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: X-API-KEY
  sources:
  - openapi/seon-tech-openapi.yml
  type: apiKey
slug: seon-tech-authentication
source_filename: seon-tech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/seon-tech-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/seon-tech-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seon-tech/refs/heads/main/authentication/seon-tech-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AML Compliance
- Device Intelligence
- Digital Footprint
- Fraud Prevention
- Identity Verification
- Risk Scoring
---
