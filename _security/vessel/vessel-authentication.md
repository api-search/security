---
api_key_in:
- header
api_specs:
- filename: vessel-platform-openapi.yml
  format: yaml
  label: Vessel Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-platform-openapi.yml
- filename: vessel-crm-openapi.yml
  format: yaml
  label: Vessel CRM API
  slug: crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-crm-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Vessel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vessel secures its APIs with apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Vessel
provider_slug: vessel
scheme_count: 4
schemes:
- description: Your Vessel API token for server-side authentication
  in: header
  name: apiToken
  parameter: vessel-api-token
  sources:
  - openapi/vessel-crm-openapi.yml
  type: apiKey
- description: Your Vessel API token for server-side authentication
  in: header
  name: apiToken
  parameter: x-vessel-api-token
  sources:
  - openapi/vessel-platform-openapi.yml
  type: apiKey
- description: User connection access token for user-scoped API calls
  in: header
  name: accessToken
  parameter: x-vessel-access-token
  sources:
  - openapi/vessel-platform-openapi.yml
  type: apiKey
- description: Temporary session token from the auth flow
  in: header
  name: sessionToken
  parameter: x-vessel-session-token
  sources:
  - openapi/vessel-platform-openapi.yml
  type: apiKey
slug: vessel-authentication
source_filename: vessel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vessel-crm-openapi.yml, openapi/vessel-platform-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiToken\n  type: apiKey\n  in: header\n  parameter: vessel-api-token\n  description: Your Vessel API token for server-side authentication\n  sources:\n  - openapi/vessel-crm-openapi.yml\n- name: apiToken\n  type: apiKey\n  in: header\n  parameter: x-vessel-api-token\n  description: Your Vessel API token for server-side authentication\n  sources:\n  - openapi/vessel-platform-openapi.yml\n- name: accessToken\n  type: apiKey\n  in: header\n  parameter: x-vessel-access-token\n  description: User connection access token for user-scoped API calls\n  sources:\n  - openapi/vessel-platform-openapi.yml\n- name: sessionToken\n  type: apiKey\n  in: header\n  parameter: x-vessel-session-token\n  description: Temporary session token from the auth flow\n  sources:\n  - openapi/vessel-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/authentication/vessel-authentication.yml
summary_line: apiKey · 4 schemes
tags:
- CRM
- Embedded Integrations
- GTM
- Integrations
- iPaaS
- Sales Engagement
- Unified API
---
