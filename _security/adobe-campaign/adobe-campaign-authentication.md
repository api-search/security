---
api_key_in:
- header
api_specs:
- filename: adobe-campaign-standard-openapi-original.yml
  format: yaml
  label: Adobe Campaign Standard API
  slug: standard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-standard-openapi-original.yml
- filename: adobe-campaign-classic-openapi-original.yml
  format: yaml
  label: Adobe Campaign Classic API
  slug: classic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-classic-openapi-original.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Adobe Campaign Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adobe Campaign secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Adobe Campaign
provider_slug: adobe-campaign
scheme_count: 3
schemes:
- description: Security token obtained from xtk:session#Logon. Must be passed alongside the session token cookie (__sessiontoken) on all authenticated requests. Tokens have a 24-hour lifecycle.
  in: header
  name: SessionToken
  parameter: X-Security-Token
  sources:
  - openapi/adobe-campaign-classic-openapi-original.yml
  type: apiKey
- bearerFormat: JWT
  description: OAuth Server-to-Server access token obtained from Adobe IMS at https://ims-na1.adobelogin.com/ims/token/v3
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/adobe-campaign-standard-openapi-original.yml
  type: http
- description: Your Adobe Developer Console API Key (Client ID).
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/adobe-campaign-standard-openapi-original.yml
  type: apiKey
slug: adobe-campaign-authentication
source_filename: adobe-campaign-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/adobe-campaign-classic-openapi-original.yml, openapi/adobe-campaign-standard-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: SessionToken\n  type: apiKey\n  in: header\n  parameter: X-Security-Token\n  description: Security token obtained from xtk:session#Logon. Must be passed alongside the\n    session token cookie (__sessiontoken) on all authenticated requests. Tokens have a 24-hour\n    lifecycle.\n  sources:\n  - openapi/adobe-campaign-classic-openapi-original.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth Server-to-Server access token obtained from Adobe IMS at https://ims-na1.adobelogin.com/ims/token/v3\n  sources:\n  - openapi/adobe-campaign-standard-openapi-original.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Your Adobe Developer Console API Key (Client\
  \ ID).\n  sources:\n  - openapi/adobe-campaign-standard-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/authentication/adobe-campaign-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
---
