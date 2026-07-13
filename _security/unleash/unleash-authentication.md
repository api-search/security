---
api_key_in:
- header
api_specs:
- filename: unleash-admin-api-openapi.yml
  format: yaml
  label: Unleash Admin API
  slug: admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unleash/refs/heads/main/openapi/unleash-admin-api-openapi.yml
- filename: unleash-client-api-openapi.yml
  format: yaml
  label: Unleash Client API
  slug: client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unleash/refs/heads/main/openapi/unleash-client-api-openapi.yml
- filename: unleash-frontend-api-openapi.yml
  format: yaml
  label: Unleash Frontend API
  slug: frontend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unleash/refs/heads/main/openapi/unleash-frontend-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Unleash Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unleash secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Unleash
provider_slug: unleash
scheme_count: 2
schemes:
- description: API key needed to access this API
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/unleash-admin-api-openapi.yml
  - openapi/unleash-client-api-openapi.yml
  - openapi/unleash-frontend-api-openapi.yml
  type: apiKey
- description: API key needed to access this API, in Bearer token format
  name: bearerToken
  scheme: bearer
  sources:
  - openapi/unleash-admin-api-openapi.yml
  - openapi/unleash-client-api-openapi.yml
  - openapi/unleash-frontend-api-openapi.yml
  type: http
slug: unleash-authentication
source_filename: unleash-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/unleash-admin-api-openapi.yml, openapi/unleash-client-api-openapi.yml, openapi/unleash-frontend-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key needed to access this API\n  sources:\n  - openapi/unleash-admin-api-openapi.yml\n  - openapi/unleash-client-api-openapi.yml\n  - openapi/unleash-frontend-api-openapi.yml\n- name: bearerToken\n  type: http\n  scheme: bearer\n  description: API key needed to access this API, in Bearer token format\n  sources:\n  - openapi/unleash-admin-api-openapi.yml\n  - openapi/unleash-client-api-openapi.yml\n  - openapi/unleash-frontend-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unleash/refs/heads/main/authentication/unleash-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Feature Flags
- Feature Management
- Progressive Delivery
- A/B Testing
- Open Source
- Developer Tools
---
