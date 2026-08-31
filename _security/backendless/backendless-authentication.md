---
api_key_in:
- header
api_specs:
- filename: backendless-cache-api-openapi.yml
  format: yaml
  label: Backendless Cache API
  slug: backendless-cache-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backendless/refs/heads/main/openapi/backendless-cache-api-openapi.yml
- filename: backendless-cloudcode-api-openapi.yml
  format: yaml
  label: Backendless CloudCode API
  slug: backendless-cloudcode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backendless/refs/heads/main/openapi/backendless-cloudcode-api-openapi.yml
- filename: backendless-counters-api-openapi.yml
  format: yaml
  label: Backendless Counters API
  slug: backendless-counters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backendless/refs/heads/main/openapi/backendless-counters-api-openapi.yml
- filename: backendless-data-api-openapi.yml
  format: yaml
  label: Backendless Data API
  slug: backendless-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backendless/refs/heads/main/openapi/backendless-data-api-openapi.yml
- filename: backendless-files-api-openapi.yml
  format: yaml
  label: Backendless Files API
  slug: backendless-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backendless/refs/heads/main/openapi/backendless-files-api-openapi.yml
- filename: backendless-geo-api-openapi.yml
  format: yaml
  label: Backendless Geo API
  slug: backendless-geo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backendless/refs/heads/main/openapi/backendless-geo-api-openapi.yml
- filename: backendless-messaging-api-openapi.yml
  format: yaml
  label: Backendless Messaging API
  slug: backendless-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backendless/refs/heads/main/openapi/backendless-messaging-api-openapi.yml
- filename: backendless-users-api-openapi.yml
  format: yaml
  label: Backendless Users API
  slug: backendless-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backendless/refs/heads/main/openapi/backendless-users-api-openapi.yml
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
- Real-Time
---
