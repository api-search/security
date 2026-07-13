---
api_key_in:
- header
- query
api_specs:
- filename: canny-openapi.yml
  format: yaml
  label: Canny REST API
  slug: v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Canny Authentication
name_suffix: Authentication
oauth_flows: []
overview: Canny secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Canny
provider_slug: canny
scheme_count: 2
schemes:
- description: 'Secret API key. Canny documents the key as a body parameter named

    `apiKey`; it is modeled here as an `apiKey` security scheme.'
  in: query
  name: apiKeyBody
  parameter: apiKey
  sources:
  - openapi/canny-openapi.yml
  type: apiKey
- in: header
  name: apiKeyHeader
  parameter: x-api-key
  sources:
  - openapi/canny-openapi.yml
  type: apiKey
slug: canny-authentication
source_filename: canny-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/canny-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyBody\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: |-\n    Secret API key. Canny documents the key as a body parameter named\n    `apiKey`; it is modeled here as an `apiKey` security scheme.\n  sources:\n  - openapi/canny-openapi.yml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/canny-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/authentication/canny-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Customer Feedback
- Product Management
- Feature Requests
- Roadmap
- Changelog
- Voice of Customer
- SaaS
---
