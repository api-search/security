---
anonymous_access: false
api_key_in:
- cookie
- header
api_specs:
- filename: openapi.json
  format: json
  label: DomScan API
  slug: domscan-api
  spec_type: OpenAPI
  url: https://domscan.net/v1/openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Domscan Authentication
name_suffix: Authentication
oauth_flows: []
overview: DomScan secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DomScan
provider_slug: domscan
scheme_count: 2
schemes:
- description: 'API key for authentication. Get yours free at https://domscan.net. Also accepts Authorization: Bearer header.'
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/domscan-openapi.json
  - openapi/domscan-swagger.json
  type: apiKey
- description: Active DomScan browser session. Used by account-management endpoints.
  in: cookie
  name: sessionCookie
  parameter: session
  sources:
  - openapi/domscan-openapi.json
  - openapi/domscan-swagger.json
  type: apiKey
slug: domscan-authentication
source_filename: domscan-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: derived\nsource: openapi/domscan-openapi.json, openapi/domscan-swagger.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: 'API key for authentication. Get yours free at https://domscan.net. Also accepts\n    Authorization: Bearer header.'\n  sources:\n  - openapi/domscan-openapi.json\n  - openapi/domscan-swagger.json\n- name: sessionCookie\n  type: apiKey\n  in: cookie\n  parameter: session\n  description: Active DomScan browser session. Used by account-management endpoints.\n  sources:\n  - openapi/domscan-openapi.json\n  - openapi/domscan-swagger.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/domscan/refs/heads/main/authentication/domscan-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Domains
- DNS
- WHOIS
- rdap
- SSL/TLS
- Email Security
- domain-valuation
- Brand Protection
- OSINT
- Threat Intelligence
- MCP
- agent-native
---
