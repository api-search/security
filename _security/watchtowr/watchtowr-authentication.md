---
api_key_in: []
api_specs:
- filename: watchtowr-platform-openapi.yml
  format: yaml
  label: watchTowr Platform Client API
  slug: watchtowr-platform-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/watchtowr/refs/heads/main/openapi/watchtowr-platform-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Watchtowr Authentication
name_suffix: Authentication
oauth_flows: []
overview: watchTowr secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: watchTowr
provider_slug: watchtowr
scheme_count: 1
schemes:
- description: API key issued from the watchTowr Platform dashboard (Settings -> API Management / Integrations -> Client API), sent as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/watchtowr-platform-openapi.yml
  type: http
slug: watchtowr-authentication
source_filename: watchtowr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/watchtowr-platform-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key issued from the watchTowr Platform dashboard (Settings -> API Management\n    / Integrations -> Client API), sent as a Bearer token.\n  sources:\n  - openapi/watchtowr-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/watchtowr/refs/heads/main/authentication/watchtowr-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Cybersecurity
- Attack Surface Management
- EASM
- Exposure Management
- Threat Intelligence
- Vulnerability Management
---
