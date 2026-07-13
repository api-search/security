---
api_key_in:
- header
api_specs:
- filename: decision-api-openapi.yml
  format: yaml
  label: AB Tasty Decision API
  slug: ab-tasty-decision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ab-tasty/refs/heads/main/openapi/decision-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ab Tasty Authentication
name_suffix: Authentication
oauth_flows: []
overview: AB Tasty secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AB Tasty
provider_slug: ab-tasty
scheme_count: 1
schemes:
- description: API key for authentication. Can be found in Flagship Platform under Parameters / Environment & Security
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/decision-api-openapi.yml
  type: apiKey
slug: ab-tasty-authentication
source_filename: ab-tasty-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/decision-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key for authentication. Can be found in Flagship Platform under Parameters\n    / Environment & Security\n  sources:\n  - openapi/decision-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ab-tasty/refs/heads/main/authentication/ab-tasty-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Aggregation
- Experimentation
- Feature Flags
- Personalization
- A/B Testing
---
