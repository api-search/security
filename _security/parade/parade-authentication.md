---
api_key_in:
- header
api_specs:
- filename: parade-digital-transactions-openapi.yaml
  format: yaml
  label: Parade Transactions API
  slug: parade-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parade/refs/heads/main/openapi/parade-digital-transactions-openapi.yaml
- filename: parade-load-sync-openapi.yaml
  format: yaml
  label: Parade Load Feed
  slug: parade-load-feed
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parade/refs/heads/main/openapi/parade-load-sync-openapi.yaml
- filename: parade-partner-webhooks-openapi.yaml
  format: yaml
  label: Parade Syndication Webhooks
  slug: parade-syndication-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parade/refs/heads/main/openapi/parade-partner-webhooks-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Parade Authentication
name_suffix: Authentication
oauth_flows: []
overview: Parade secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Parade
provider_slug: parade
scheme_count: 1
schemes:
- description: Contact us to get an authorization token
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/parade-digital-transactions-openapi.yaml
  - openapi/parade-load-sync-openapi.yaml
  type: apiKey
slug: parade-authentication
source_filename: parade-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/parade-digital-transactions-openapi.yaml, openapi/parade-load-sync-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Contact us to get an authorization token\n  sources:\n  - openapi/parade-digital-transactions-openapi.yaml\n  - openapi/parade-load-sync-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parade/refs/heads/main/authentication/parade-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Freight
- Logistics
- Trucking
- Supply Chain
- Capacity Management
- Freight Brokerage
- Transportation
- Load Board
- Artificial Intelligence
---
