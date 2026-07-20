---
api_key_in:
- header
api_specs:
- filename: diligent-openapi-original.json
  format: json
  label: Diligent API
  slug: diligent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diligent/refs/heads/main/openapi/diligent-openapi-original.json
- filename: diligent-remediation-openapi.json
  format: json
  label: Diligent Remediation API (Beta)
  slug: diligent-remediation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diligent/refs/heads/main/openapi/diligent-remediation-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Diligent Authentication
name_suffix: Authentication
oauth_flows: []
overview: Diligent secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Diligent
provider_slug: diligent
scheme_count: 1
schemes:
- in: header
  name: xApiKey
  parameter: X-API-KEY
  sources:
  - openapi/diligent-openapi-original.json
  - openapi/diligent-remediation-openapi.json
  type: apiKey
slug: diligent-authentication
source_filename: diligent-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/diligent-openapi-original.json, openapi/diligent-remediation-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: xApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/diligent-openapi-original.json\n  - openapi/diligent-remediation-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diligent/refs/heads/main/authentication/diligent-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Compliance
- RegTech
- KYC
- AML
- Financial Crime
- Due Diligence
- Screening
- Sanctions
- Monitoring
- Artificial Intelligence
- Fintech
- Webhooks
---
