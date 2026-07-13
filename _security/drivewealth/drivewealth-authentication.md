---
api_key_in:
- header
api_specs:
- filename: dw-openapi
  format: yaml
  label: DriveWealth REST API
  slug: drivewealth-rest-api
  spec_type: OpenAPI
  url: https://github.com/DriveWealth/dw-openapi
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Drivewealth Authentication
name_suffix: Authentication
oauth_flows: []
overview: DriveWealth secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DriveWealth
provider_slug: drivewealth
scheme_count: 3
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/drivewealth-rest-openapi.yml
  type: http
- in: header
  name: dwAppKey
  parameter: dw-client-app-key
  sources:
  - openapi/drivewealth-rest-openapi.yml
  type: apiKey
- in: header
  name: sessionToken
  parameter: dw-auth-token
  sources:
  - openapi/drivewealth-rest-openapi.yml
  type: apiKey
slug: drivewealth-authentication
source_filename: drivewealth-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/drivewealth-rest-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/drivewealth-rest-openapi.yml\n- name: dwAppKey\n  type: apiKey\n  in: header\n  parameter: dw-client-app-key\n  sources:\n  - openapi/drivewealth-rest-openapi.yml\n- name: sessionToken\n  type: apiKey\n  in: header\n  parameter: dw-auth-token\n  sources:\n  - openapi/drivewealth-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drivewealth/refs/heads/main/authentication/drivewealth-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Brokerage-as-a-Service
- Embedded Investing
- Fractional Shares
- Trading
- Fintech
- Equities
- ETFs
- Options
- Fixed Income
- Mutual Funds
- Portfolio Management
- Account Opening
- KYC
- Financial Services
---
