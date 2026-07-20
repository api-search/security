---
api_key_in:
- cookie
- header
- query
api_specs:
- filename: extole-integration-consumer-to-extole-openapi.json
  format: json
  label: Extole Integration API - Consumer to Extole
  slug: extole-integration-api-consumer-to-extole
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extole/refs/heads/main/openapi/extole-integration-consumer-to-extole-openapi.json
- filename: extole-integration-server-to-extole-openapi.json
  format: json
  label: Extole Integration API - Server to Extole
  slug: extole-integration-api-server-to-extole
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extole/refs/heads/main/openapi/extole-integration-server-to-extole-openapi.json
- filename: extole-management-openapi.json
  format: json
  label: Extole Management API
  slug: extole-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extole/refs/heads/main/openapi/extole-management-openapi.json
- filename: extole-management-expert-openapi.json
  format: json
  label: Extole Management Expert API
  slug: extole-management-expert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extole/refs/heads/main/openapi/extole-management-expert-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Extole Authentication
name_suffix: Authentication
oauth_flows: []
overview: Extole secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Extole
provider_slug: extole
scheme_count: 3
schemes:
- in: cookie
  name: COOKIE
  parameter: extole_token
  sources:
  - openapi/extole-integration-consumer-to-extole-openapi.json
  - openapi/extole-integration-server-to-extole-openapi.json
  - openapi/extole-management-expert-openapi.json
  - openapi/extole-management-openapi.json
  type: apiKey
- in: header
  name: HEADER
  parameter: Authorization
  sources:
  - openapi/extole-integration-consumer-to-extole-openapi.json
  - openapi/extole-integration-server-to-extole-openapi.json
  - openapi/extole-management-expert-openapi.json
  - openapi/extole-management-openapi.json
  type: apiKey
- in: query
  name: QUERY
  parameter: access_token
  sources:
  - openapi/extole-integration-consumer-to-extole-openapi.json
  - openapi/extole-integration-server-to-extole-openapi.json
  - openapi/extole-management-expert-openapi.json
  - openapi/extole-management-openapi.json
  type: apiKey
slug: extole-authentication
source_filename: extole-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/extole-integration-consumer-to-extole-openapi.json, openapi/extole-integration-server-to-extole-openapi.json,\n  openapi/extole-management-expert-openapi.json, openapi/extole-management-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\n  - header\n  - query\nschemes:\n- name: COOKIE\n  type: apiKey\n  in: cookie\n  parameter: extole_token\n  sources:\n  - openapi/extole-integration-consumer-to-extole-openapi.json\n  - openapi/extole-integration-server-to-extole-openapi.json\n  - openapi/extole-management-expert-openapi.json\n  - openapi/extole-management-openapi.json\n- name: HEADER\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/extole-integration-consumer-to-extole-openapi.json\n  - openapi/extole-integration-server-to-extole-openapi.json\n  - openapi/extole-management-expert-openapi.json\n  - openapi/extole-management-openapi.json\n- name: QUERY\n  type: apiKey\n\
  \  in: query\n  parameter: access_token\n  sources:\n  - openapi/extole-integration-consumer-to-extole-openapi.json\n  - openapi/extole-integration-server-to-extole-openapi.json\n  - openapi/extole-management-expert-openapi.json\n  - openapi/extole-management-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/extole/refs/heads/main/authentication/extole-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Referral Marketing
- Advocacy
- Loyalty
- Rewards
- Marketing
- Customer Acquisition
- SaaS
---
