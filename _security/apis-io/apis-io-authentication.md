---
api_key_in:
- header
api_specs:
- filename: apis-io-v1-openapi.yml
  format: yaml
  label: APIs.io Search API
  slug: search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-v1-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Apis Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: APIs.io secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: APIs.io
provider_slug: apis-io
scheme_count: 2
schemes:
- in: header
  name: api_key
  parameter: x-api-key
  sources:
  - openapi/apis-io-search-openapi.yaml
  type: apiKey
- description: Optional in v1. Defined so metering/rate-tiers can be enabled later without a breaking change.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/apis-io-v1-openapi.yml
  type: apiKey
slug: apis-io-authentication
source_filename: apis-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apis-io-search-openapi.yaml, openapi/apis-io-v1-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/apis-io-search-openapi.yaml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Optional in v1. Defined so metering/rate-tiers can be enabled later without a\n    breaking change.\n  sources:\n  - openapi/apis-io-v1-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/authentication/apis-io-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- API Aggregation
- API Directory
- API Discovery
- API Indexing
- API Rating
- API Search
- APIs.json
- Search Engine
---
