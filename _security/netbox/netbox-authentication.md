---
api_key_in:
- cookie
- header
api_specs:
- filename: netbox-openapi.yml
  format: yaml
  label: NetBox REST API
  slug: netbox-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox/refs/heads/main/openapi/netbox-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Netbox Authentication
name_suffix: Authentication
oauth_flows: []
overview: NetBox secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: NetBox
provider_slug: netbox
scheme_count: 2
schemes:
- in: cookie
  name: cookieAuth
  parameter: sessionid
  sources:
  - openapi/netbox-openapi.yml
  type: apiKey
- description: '`Token <token>` (v1) or `Bearer <key>.<token>` (v2)'
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/netbox-openapi.yml
  type: apiKey
slug: netbox-authentication
source_filename: netbox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/netbox-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: sessionid\n  sources:\n  - openapi/netbox-openapi.yml\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: '`Token <token>` (v1) or `Bearer <key>.<token>` (v2)'\n  sources:\n  - openapi/netbox-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netbox/refs/heads/main/authentication/netbox-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Data Center
- DCIM
- Infrastructure as Code
- IPAM
- Network Automation
- Network Management
- Open Source
- Source of Truth
---
