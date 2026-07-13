---
api_key_in:
- header
api_specs:
- filename: watchguard-cloud-platform-openapi.yml
  format: yaml
  label: WatchGuard Cloud Platform API
  slug: watchguard-cloud-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/watchguard/refs/heads/main/openapi/watchguard-cloud-platform-openapi.yml
- filename: watchguard-endpoint-security-openapi.yml
  format: yaml
  label: WatchGuard Endpoint Security Management API
  slug: watchguard-endpoint-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/watchguard/refs/heads/main/openapi/watchguard-endpoint-security-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Watchguard Authentication
name_suffix: Authentication
oauth_flows: []
overview: WatchGuard secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: WatchGuard
provider_slug: watchguard
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 access token obtained from the WatchGuard Authentication API.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/watchguard-cloud-platform-openapi.yml
  - openapi/watchguard-endpoint-security-openapi.yml
  type: http
- description: API key from the WatchGuard Cloud Managed Access page.
  in: header
  name: apiKeyAuth
  parameter: WatchGuard-API-Key
  sources:
  - openapi/watchguard-cloud-platform-openapi.yml
  - openapi/watchguard-endpoint-security-openapi.yml
  type: apiKey
slug: watchguard-authentication
source_filename: watchguard-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/watchguard-cloud-platform-openapi.yml, openapi/watchguard-endpoint-security-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 access token obtained from the WatchGuard Authentication API.\n  sources:\n  - openapi/watchguard-cloud-platform-openapi.yml\n  - openapi/watchguard-endpoint-security-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: WatchGuard-API-Key\n  description: API key from the WatchGuard Cloud Managed Access page.\n  sources:\n  - openapi/watchguard-cloud-platform-openapi.yml\n  - openapi/watchguard-endpoint-security-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/watchguard/refs/heads/main/authentication/watchguard-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Cloud Security
- Endpoint Security
- Firewall
- MFA
- Network Security
- Zero Trust
---
