---
api_key_in:
- header
api_specs:
- filename: backendless-openapi.yml
  format: yaml
  label: Backendless Data Service API
  slug: data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backendless/refs/heads/main/openapi/backendless-openapi.yml
- filename: backendless-openapi.yml
  format: yaml
  label: Backendless User Service API
  slug: users
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backendless/refs/heads/main/openapi/backendless-openapi.yml
- filename: backendless-openapi.yml
  format: yaml
  label: Backendless File Service API
  slug: files
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backendless/refs/heads/main/openapi/backendless-openapi.yml
- filename: backendless-openapi.yml
  format: yaml
  label: Backendless Messaging and Push API
  slug: messaging
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backendless/refs/heads/main/openapi/backendless-openapi.yml
- filename: backendless-openapi.yml
  format: yaml
  label: Backendless Geo Service API
  slug: geo
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backendless/refs/heads/main/openapi/backendless-openapi.yml
- filename: backendless-openapi.yml
  format: yaml
  label: Backendless Cache and Atomic Counters API
  slug: cache-counters
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backendless/refs/heads/main/openapi/backendless-openapi.yml
- filename: backendless-openapi.yml
  format: yaml
  label: Backendless Cloud Code API
  slug: cloud-code
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backendless/refs/heads/main/openapi/backendless-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Backendless Authentication
name_suffix: Authentication
oauth_flows: []
overview: Backendless secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Backendless
provider_slug: backendless
scheme_count: 1
schemes:
- description: Session token returned by POST /users/login. Required on operations that run in the context of an authenticated user. The application id and REST API key that scope every request are carried in the server URL path rather than as a security scheme.
  in: header
  name: userToken
  parameter: user-token
  sources:
  - openapi/backendless-openapi.yml
  type: apiKey
slug: backendless-authentication
source_filename: backendless-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/backendless-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: userToken\n  type: apiKey\n  in: header\n  parameter: user-token\n  description: Session token returned by POST /users/login. Required on operations that run\n    in the context of an authenticated user. The application id and REST API key that scope\n    every request are carried in the server URL path rather than as a security scheme.\n  sources:\n  - openapi/backendless-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/backendless/refs/heads/main/authentication/backendless-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- BaaS
- Backend as a Service
- Visual Development
- Low Code
- Database
- Realtime
---
