---
api_key_in:
- query
api_specs:
- filename: brickwork-openapi.yml
  format: yaml
  label: Brickwork API v3
  slug: brickwork-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brickwork/refs/heads/main/openapi/brickwork-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Brickwork Authentication
name_suffix: Authentication
oauth_flows: []
overview: Brickwork secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Brickwork
provider_slug: brickwork
scheme_count: 1
schemes:
- description: Company API key passed as the api_key query parameter.
  in: query
  name: apiKeyAuth
  parameter: api_key
  sources:
  - openapi/brickwork-openapi.yml
  type: apiKey
slug: brickwork-authentication
source_filename: brickwork-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/brickwork-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Company API key passed as the api_key query parameter.\n  sources:\n  - openapi/brickwork-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brickwork/refs/heads/main/authentication/brickwork-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Consumer
- Retail
- Omnichannel
- Store Locator
- Appointments
- Events
- Location Data
- CMS
---
