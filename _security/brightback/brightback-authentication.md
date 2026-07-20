---
api_key_in:
- header
api_specs:
- filename: brightback-retention-openapi.yml
  format: yaml
  label: Brightback Pre-cancel API
  slug: brightback-pre-cancel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightback/refs/heads/main/openapi/brightback-retention-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Brightback Authentication
name_suffix: Authentication
oauth_flows: []
overview: brightback secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: brightback
provider_slug: brightback
scheme_count: 2
schemes:
- description: HMAC-SHA-512 signature computed over the request payload plus an ISO8601 timestamp, using the account's Brightback-issued private key.
  in: header
  name: hmacSignature
  parameter: Signature
  sources:
  - openapi/brightback-retention-openapi.yml
  type: apiKey
- description: The Brightback-issued public key identifying the signing account.
  in: header
  name: hmacPublicKey
  parameter: Signature-Public-Key
  sources:
  - openapi/brightback-retention-openapi.yml
  type: apiKey
slug: brightback-authentication
source_filename: brightback-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/brightback-retention-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmacSignature\n  type: apiKey\n  in: header\n  parameter: Signature\n  description: HMAC-SHA-512 signature computed over the request payload plus an ISO8601 timestamp,\n    using the account's Brightback-issued private key.\n  sources:\n  - openapi/brightback-retention-openapi.yml\n- name: hmacPublicKey\n  type: apiKey\n  in: header\n  parameter: Signature-Public-Key\n  description: The Brightback-issued public key identifying the signing account.\n  sources:\n  - openapi/brightback-retention-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brightback/refs/heads/main/authentication/brightback-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Churn Prevention
- Customer Retention
- Subscriptions
- Cancellation
- SaaS
---
