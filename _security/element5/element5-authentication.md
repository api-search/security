---
api_key_in:
- header
api_specs:
- filename: element5-openapi-original.json
  format: json
  label: Element5 API
  slug: element5-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/element5/refs/heads/main/openapi/element5-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Element5 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Element5 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Element5
provider_slug: element5
scheme_count: 1
schemes:
- description: API key provided by Element5 to authenticate and authorize the Element5 APIs
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/element5-openapi-original.json
  type: apiKey
slug: element5-authentication
source_filename: element5-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/element5-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key provided by Element5 to authenticate and authorize the Element5 APIs\n  sources:\n  - openapi/element5-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/element5/refs/heads/main/authentication/element5-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Healthcare
- Revenue Cycle Management
- Post-Acute Care
- Workflow Automation
- Eligibility Verification
- Prior Authorization
- Claims Processing
- Webhooks
- Artificial Intelligence
---
