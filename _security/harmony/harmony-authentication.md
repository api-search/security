---
api_key_in:
- header
api_specs:
- filename: harmony-service-desk-openapi.json
  format: json
  label: Harmony Service Desk API
  slug: harmony-service-desk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harmony/refs/heads/main/openapi/harmony-service-desk-openapi.json
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Harmony Authentication
name_suffix: Authentication
oauth_flows: []
overview: Harmony secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Harmony
provider_slug: harmony
scheme_count: 2
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/harmony-service-desk-openapi.json
  type: http
- format: AccessKey <token>
  in: header
  name: AccessKey
  parameter_name: Authorization
  provisioning: Settings > API Keys > Generate New API Key (shown once)
  source: https://docs.harmony.io/api-references/api-documentation/introduction
  type: apiKey
slug: harmony-authentication
source_filename: harmony-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/harmony-service-desk-openapi.json\ndocs: https://docs.harmony.io/api-references/api-documentation/introduction\nsummary:\n  types:\n  - http\n  - apiKey\n  api_key_in:\n  - header\n  notes: >-\n    The published OpenAPI declares a single HTTP bearer scheme (HTTPBearer). The developer docs\n    document the live scheme as an AccessKey token passed in the Authorization header\n    (`Authorization: AccessKey <token>`). Tokens are generated per organization under\n    Settings > API Keys and are shown once. The API base URL is per-tenant:\n    https://<customer_subdomain>.harmony.io.\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/harmony-service-desk-openapi.json\n- name: AccessKey\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  format: 'AccessKey <token>'\n  source: https://docs.harmony.io/api-references/api-documentation/introduction\n  provisioning: Settings >\
  \ API Keys > Generate New API Key (shown once)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harmony/refs/heads/main/authentication/harmony-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- IT Service Management
- Service Desk
- Ticketing
- Enterprise Service Management
- AI Agents
- IT Automation
- Help Desk
- Identity
- Company
---
