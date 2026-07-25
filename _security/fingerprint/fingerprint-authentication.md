---
api_key_in:
- header
- query
api_specs:
- filename: fingerprint-event-search-api-openapi.yml
  format: yaml
  label: Fingerprint Event Search API
  slug: fingerprint-event-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fingerprint/refs/heads/main/openapi/fingerprint-event-search-api-openapi.yml
- filename: fingerprint-events-api-openapi.yml
  format: yaml
  label: Fingerprint Events API
  slug: fingerprint-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fingerprint/refs/heads/main/openapi/fingerprint-events-api-openapi.yml
- filename: fingerprint-related-visitors-api-openapi.yml
  format: yaml
  label: Fingerprint Related Visitors API
  slug: fingerprint-related-visitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fingerprint/refs/heads/main/openapi/fingerprint-related-visitors-api-openapi.yml
- filename: fingerprint-visitors-api-openapi.yml
  format: yaml
  label: Fingerprint Visitors API
  slug: fingerprint-visitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fingerprint/refs/heads/main/openapi/fingerprint-visitors-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Fingerprint Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fingerprint secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Fingerprint
provider_slug: fingerprint
scheme_count: 2
schemes:
- in: header
  name: ApiKeyHeader
  parameter: Auth-API-Key
  sources:
  - openapi/fingerprint-openapi.yml
  type: apiKey
- in: query
  name: ApiKeyQuery
  parameter: api_key
  sources:
  - openapi/fingerprint-openapi.yml
  type: apiKey
slug: fingerprint-authentication
source_filename: fingerprint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fingerprint-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Auth-API-Key\n  sources:\n  - openapi/fingerprint-openapi.yml\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/fingerprint-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fingerprint/refs/heads/main/authentication/fingerprint-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Device Identification
- Fraud Prevention
- Bot Detection
- Smart Signals
- Identity
---
