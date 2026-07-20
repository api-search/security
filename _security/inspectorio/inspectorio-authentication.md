---
api_key_in:
- header
api_specs:
- filename: inspectorio-qrm-openapi.json
  format: json
  label: Inspectorio Quality Risk Management API
  slug: inspectorio-quality-risk-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inspectorio/refs/heads/main/openapi/inspectorio-qrm-openapi.json
- filename: inspectorio-rsc-openapi.json
  format: json
  label: Inspectorio Responsible Sourcing & Compliance API
  slug: inspectorio-responsible-sourcing-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inspectorio/refs/heads/main/openapi/inspectorio-rsc-openapi.json
- filename: inspectorio-fms-openapi.json
  format: json
  label: Inspectorio File Management API
  slug: inspectorio-file-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inspectorio/refs/heads/main/openapi/inspectorio-fms-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Inspectorio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Inspectorio secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Inspectorio
provider_slug: inspectorio
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: apiKey
  sources:
  - openapi/inspectorio-qrm-openapi.json
  - openapi/inspectorio-rsc-openapi.json
  type: apiKey
slug: inspectorio-authentication
source_filename: inspectorio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/inspectorio-qrm-openapi.json, openapi/inspectorio-rsc-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: apiKey\n  sources:\n  - openapi/inspectorio-qrm-openapi.json\n  - openapi/inspectorio-rsc-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inspectorio/refs/heads/main/authentication/inspectorio-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Supply Chain
- Quality Management
- Compliance
- Responsible Sourcing
- Traceability
- Manufacturing
- Retail
- Lab Testing
- Company
---
