---
api_key_in:
- header
api_specs:
- filename: demisto-openapi-original.json
  format: json
  label: Demisto REST API
  slug: demisto-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demisto/refs/heads/main/openapi/demisto-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Demisto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Demisto secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Demisto
provider_slug: demisto
scheme_count: 3
schemes:
- description: Primary API key (legacy Demisto / XSOAR 6.x). XSOAR 8+ uses the API-Key / API-Key-ID pair.
  in: header
  name: api_key
  parameter: Authorization
  sources:
  - openapi/demisto-openapi-original.json
  type: apiKey
- in: header
  name: csrf_token
  parameter: X-XSRF-TOKEN
  sources:
  - openapi/demisto-openapi-original.json
  type: apiKey
- description: Advanced API-Key-ID for XSOAR 8+ / XSIAM tenants.
  in: header
  name: x-xdr-auth-id
  parameter: x-xdr-auth-id
  sources:
  - openapi/demisto-openapi-original.json
  type: apiKey
slug: demisto-authentication
source_filename: demisto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/demisto-openapi-original.json\ndocs: https://docs-cortex.paloaltonetworks.com/r/Cortex-XSOAR/8/Cortex-XSOAR-Administrator-Guide/Get-Started-with-APIs\nnote: >-\n  The Demisto REST API (now Cortex XSOAR, Palo Alto Networks) authenticates with an API key.\n  Legacy Demisto / XSOAR 6.x sends the key in the `Authorization` header. XSOAR 8+ / XSIAM\n  add an advanced-key model that pairs an `API-Key` with an `API-Key-ID` (sent as `x-xdr-auth-id`)\n  and a `csrf_token` (`X-XSRF-TOKEN`). Keys are generated in the web UI under\n  Settings > Integrations > API Keys. The API is instance-scoped (self-hosted server or SaaS tenant),\n  so there is no OAuth flow and no scope surface.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Primary API key (legacy Demisto / XSOAR 6.x). XSOAR 8+ uses the API-Key / API-Key-ID pair.\n\
  \  sources:\n  - openapi/demisto-openapi-original.json\n- name: csrf_token\n  type: apiKey\n  in: header\n  parameter: X-XSRF-TOKEN\n  sources:\n  - openapi/demisto-openapi-original.json\n- name: x-xdr-auth-id\n  type: apiKey\n  in: header\n  parameter: x-xdr-auth-id\n  description: Advanced API-Key-ID for XSOAR 8+ / XSIAM tenants.\n  sources:\n  - openapi/demisto-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/demisto/refs/heads/main/authentication/demisto-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Security
- SOAR
- Incident Response
- Threat Intelligence
- Security Automation
---
