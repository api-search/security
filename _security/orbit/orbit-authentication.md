---
api_key_in:
- query
api_specs:
- filename: swagger.json
  format: json
  label: Orbit REST API
  slug: orbit-rest-api
  spec_type: OpenAPI
  url: https://app.orbit.love/api-docs/v1/swagger.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Orbit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orbit secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Orbit
provider_slug: orbit
scheme_count: 2
schemes:
- description: Provide a Authorization header with format 'Bearer <api_key>'. This is the recommended approach. Make sure to include the 'Bearer' part in the text box here.
  name: bearer
  scheme: bearer
  sources:
  - openapi/orbit-rest-api-openapi.yml
  type: http
- description: Provide the API key in a query param called api_key. This is the least secure method, please use only for testing.
  in: query
  name: api_key
  parameter: api_key
  sources:
  - openapi/orbit-rest-api-openapi.yml
  type: apiKey
slug: orbit-authentication
source_filename: orbit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/orbit-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: Provide a Authorization header with format 'Bearer <api_key>'. This is the recommended\n    approach. Make sure to include the 'Bearer' part in the text box here.\n  sources:\n  - openapi/orbit-rest-api-openapi.yml\n- name: api_key\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Provide the API key in a query param called api_key. This is the least secure\n    method, please use only for testing.\n  sources:\n  - openapi/orbit-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orbit/refs/heads/main/authentication/orbit-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Developer Relations
- Community Intelligence
- DevRel
- Community Management
- Member Tracking
- Community Analytics
- Open Source
- Developer Engagement
---
