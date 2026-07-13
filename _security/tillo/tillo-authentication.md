---
api_key_in:
- header
api_specs:
- filename: tillo-gift-card-openapi.yml
  format: yaml
  label: Tillo Gift Card API
  slug: tillo-gift-card-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tillo/refs/heads/main/openapi/tillo-gift-card-openapi.yml
- filename: tillo-gift-card-openapi.yml
  format: yaml
  label: Tillo Float Management API
  slug: tillo-float-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tillo/refs/heads/main/openapi/tillo-gift-card-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tillo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tillo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tillo
provider_slug: tillo
scheme_count: 1
schemes:
- description: HMAC-SHA256 signature. Signature is built from API Key, HTTP Method, Endpoint, Client Request ID, Brand Identifier, and UTC Timestamp (ms), concatenated with hyphens and hashed with your API Secret.
  in: header
  name: HMACAuth
  parameter: Authorization
  sources:
  - openapi/tillo-gift-card-openapi.yml
  type: apiKey
slug: tillo-authentication
source_filename: tillo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tillo-gift-card-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: HMACAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: HMAC-SHA256 signature. Signature is built from API Key, HTTP Method, Endpoint,\n    Client Request ID, Brand Identifier, and UTC Timestamp (ms), concatenated with hyphens and\n    hashed with your API Secret.\n  sources:\n  - openapi/tillo-gift-card-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tillo/refs/heads/main/authentication/tillo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Finance
- Gift Cards
- Payments
- Rewards
- Incentives
---
