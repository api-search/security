---
api_key_in:
- query
api_specs:
- filename: marvel-openapi.yml
  format: yaml
  label: Marvel Comics API
  slug: marvel-comics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marvel/refs/heads/main/openapi/marvel-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Marvel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Marvel secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Marvel
provider_slug: marvel
scheme_count: 3
schemes:
- description: Public API key issued from the Marvel Developer Portal.
  in: query
  name: apiKeyAuth
  parameter: apikey
  sources:
  - openapi/marvel-openapi.yml
  type: apiKey
- description: Timestamp (or other long string) used in the hash computation.
  in: query
  name: timestampAuth
  parameter: ts
  sources:
  - openapi/marvel-openapi.yml
  type: apiKey
- description: MD5 hash of ts + private key + public key.
  in: query
  name: hashAuth
  parameter: hash
  sources:
  - openapi/marvel-openapi.yml
  type: apiKey
slug: marvel-authentication
source_filename: marvel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/marvel-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: Public API key issued from the Marvel Developer Portal.\n  sources:\n  - openapi/marvel-openapi.yml\n- name: timestampAuth\n  type: apiKey\n  in: query\n  parameter: ts\n  description: Timestamp (or other long string) used in the hash computation.\n  sources:\n  - openapi/marvel-openapi.yml\n- name: hashAuth\n  type: apiKey\n  in: query\n  parameter: hash\n  description: MD5 hash of ts + private key + public key.\n  sources:\n  - openapi/marvel-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marvel/refs/heads/main/authentication/marvel-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Characters
- Comics
- Creators
- Entertainment
- Events
- Media
- Series
- Stories
---
