---
api_key_in:
- header
api_specs:
- filename: parade-available-trucks-api-openapi.yml
  format: yaml
  label: Parade Available Trucks API
  slug: parade-available-trucks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parade/refs/heads/main/openapi/parade-available-trucks-api-openapi.yml
- filename: parade-bookings-api-openapi.yml
  format: yaml
  label: Parade Bookings API
  slug: parade-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parade/refs/heads/main/openapi/parade-bookings-api-openapi.yml
- filename: parade-carrier-onboarding-status-api-openapi.yml
  format: yaml
  label: Parade Carrier Onboarding Status API
  slug: parade-carrier-onboarding-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parade/refs/heads/main/openapi/parade-carrier-onboarding-status-api-openapi.yml
- filename: parade-carrier-synchronization-api-openapi.yml
  format: yaml
  label: Parade Carrier Synchronization API
  slug: parade-carrier-synchronization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parade/refs/heads/main/openapi/parade-carrier-synchronization-api-openapi.yml
- filename: parade-digital-conversion-api-openapi.yml
  format: yaml
  label: Parade Digital Conversion API
  slug: parade-digital-conversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parade/refs/heads/main/openapi/parade-digital-conversion-api-openapi.yml
- filename: parade-load-synchronization-api-openapi.yml
  format: yaml
  label: Parade Load Synchronization API
  slug: parade-load-synchronization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parade/refs/heads/main/openapi/parade-load-synchronization-api-openapi.yml
- filename: parade-quotes-api-openapi.yml
  format: yaml
  label: Parade Quotes API
  slug: parade-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parade/refs/heads/main/openapi/parade-quotes-api-openapi.yml
- filename: parade-search-api-openapi.yml
  format: yaml
  label: Parade Search API
  slug: parade-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parade/refs/heads/main/openapi/parade-search-api-openapi.yml
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
