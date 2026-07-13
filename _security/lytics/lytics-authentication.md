---
api_key_in:
- header
- query
api_specs:
- filename: lytics-rest-api-openapi.yml
  format: yaml
  label: Lytics REST API
  slug: lytics-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lytics/refs/heads/main/openapi/lytics-rest-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Lytics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lytics secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lytics
provider_slug: lytics
scheme_count: 2
schemes:
- description: Lytics API key passed as a query parameter. Obtain your API key from the Lytics account settings.
  in: query
  name: ApiKeyQuery
  parameter: key
  sources:
  - openapi/lytics-rest-api-openapi.yml
  type: apiKey
- description: Lytics API key passed as an Authorization header value.
  in: header
  name: ApiKeyHeader
  parameter: Authorization
  sources:
  - openapi/lytics-rest-api-openapi.yml
  type: apiKey
slug: lytics-authentication
source_filename: lytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lytics-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  description: Lytics API key passed as a query parameter. Obtain your API key from the Lytics\n    account settings.\n  sources:\n  - openapi/lytics-rest-api-openapi.yml\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Lytics API key passed as an Authorization header value.\n  sources:\n  - openapi/lytics-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lytics/refs/heads/main/authentication/lytics-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Customer Data Platform
- CDP
- Personalization
- Segmentation
- User Profiles
- Behavioral Analytics
- Content Affinity
- Real-Time Data
- Marketing Automation
- Audience Activation
---
