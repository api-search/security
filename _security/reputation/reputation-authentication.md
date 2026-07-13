---
api_key_in:
- header
api_specs:
- filename: reputation-api-openapi.yml
  format: yaml
  label: Reputation API
  slug: reputation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Reputation Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reputation secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Reputation
provider_slug: reputation
scheme_count: 1
schemes:
- description: API key for authentication. For agency accounts, also include X-TENANT-ID header.
  in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/reputation-api-openapi.yml
  type: apiKey
slug: reputation-authentication
source_filename: reputation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/reputation-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: API key for authentication. For agency accounts, also include X-TENANT-ID header.\n  sources:\n  - openapi/reputation-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/authentication/reputation-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Reputation Management
- Online Reviews
- Business Listings
- Surveys
- Social Listening
- Competitive Intelligence
- Customer Experience
- Local SEO
---
