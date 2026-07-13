---
api_key_in:
- header
api_specs:
- filename: seon-openapi.yml
  format: yaml
  label: SEON Fraud API
  slug: fraud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seon/refs/heads/main/openapi/seon-openapi.yml
- filename: seon-openapi.yml
  format: yaml
  label: SEON Email API
  slug: email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seon/refs/heads/main/openapi/seon-openapi.yml
- filename: seon-openapi.yml
  format: yaml
  label: SEON Phone API
  slug: phone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seon/refs/heads/main/openapi/seon-openapi.yml
- filename: seon-openapi.yml
  format: yaml
  label: SEON IP API
  slug: ip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seon/refs/heads/main/openapi/seon-openapi.yml
- filename: seon-openapi.yml
  format: yaml
  label: SEON AML API
  slug: aml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seon/refs/heads/main/openapi/seon-openapi.yml
- filename: seon-openapi.yml
  format: yaml
  label: SEON Scoring / Labels API
  slug: transaction-label-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seon/refs/heads/main/openapi/seon-openapi.yml
- filename: seon-openapi.yml
  format: yaml
  label: SEON Device Fingerprint
  slug: device-fingerprint
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seon/refs/heads/main/openapi/seon-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Seon Authentication
name_suffix: Authentication
oauth_flows: []
overview: SEON secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SEON
provider_slug: seon
scheme_count: 1
schemes:
- description: SEON license key sent as the X-API-KEY request header.
  in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/seon-openapi.yml
  type: apiKey
slug: seon-authentication
source_filename: seon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/seon-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: SEON license key sent as the X-API-KEY request header.\n  sources:\n  - openapi/seon-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seon/refs/heads/main/authentication/seon-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Fraud Prevention
- Risk Scoring
- Digital Footprint
- AML
- Identity
---
