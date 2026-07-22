---
api_key_in:
- cookie
- header
api_specs:
- filename: netbox-labs-openapi-original.json
  format: json
  label: NetBox REST API
  slug: netbox-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox-labs/refs/heads/main/openapi/netbox-labs-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Netbox Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: NetBox Labs secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: NetBox Labs
provider_slug: netbox-labs
scheme_count: 2
schemes:
- in: cookie
  name: cookieAuth
  parameter: sessionid
  sources:
  - openapi/netbox-labs-openapi-original.json
  type: apiKey
- description: '`Token <token>` (v1) or `Bearer <key>.<token>` (v2)'
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/netbox-labs-openapi-original.json
  type: apiKey
slug: netbox-labs-authentication
source_filename: netbox-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/netbox-labs-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: sessionid\n  sources:\n  - openapi/netbox-labs-openapi-original.json\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: '`Token <token>` (v1) or `Bearer <key>.<token>` (v2)'\n  sources:\n  - openapi/netbox-labs-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netbox-labs/refs/heads/main/authentication/netbox-labs-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Networking
- DCIM
- IPAM
- Infrastructure
- Source of Truth
- Network Automation
- OpenAPI
- MCP
---
