---
api_key_in:
- header
api_specs:
- filename: varonis-datalert-openapi.yml
  format: yaml
  label: Varonis DatAlert API
  slug: varonis-datalert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varonis/refs/heads/main/openapi/varonis-datalert-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Varonis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Varonis secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Varonis
provider_slug: varonis
scheme_count: 1
schemes:
- description: API key for authenticating with the Varonis DatAlert API. Generate an API key from the Varonis Web Interface under Configuration, then API Keys. The key must have the Threat Detection Integrator role.
  in: header
  name: apiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/varonis-datalert-openapi.yml
  type: apiKey
slug: varonis-authentication
source_filename: varonis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/varonis-datalert-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key for authenticating with the Varonis DatAlert API. Generate an API key\n    from the Varonis Web Interface under Configuration, then API Keys. The key must have the\n    Threat Detection Integrator role.\n  sources:\n  - openapi/varonis-datalert-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/varonis/refs/heads/main/authentication/varonis-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cloud Security
- Compliance
- Data Analytics
- Data Governance
- Data Security
- Threat Detection
---
