---
anonymous_access: false
api_key_in:
- cookie
- header
api_specs:
- filename: darwin-so-account-api-openapi.yml
  format: yaml
  label: Darwin Technologies, Inc. Account API
  slug: darwin-so-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/darwin-so/openapi/darwin-so-account-api-openapi.yml
- filename: darwin-so-accounts-api-openapi.yml
  format: yaml
  label: Darwin Technologies, Inc. Accounts API
  slug: darwin-so-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/darwin-so/openapi/darwin-so-accounts-api-openapi.yml
- filename: darwin-so-act-api-openapi.yml
  format: yaml
  label: Darwin Technologies, Inc. Act API
  slug: darwin-so-act-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/darwin-so/openapi/darwin-so-act-api-openapi.yml
- filename: darwin-so-search-api-openapi.yml
  format: yaml
  label: Darwin Technologies, Inc. Search API
  slug: darwin-so-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/darwin-so/openapi/darwin-so-search-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Darwin Technologies, Inc. Authentication
name_suffix: Authentication
oauth_flows: []
overview: Darwin Technologies, Inc. secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Darwin Technologies, Inc.
provider_slug: darwin-so
scheme_count: 3
schemes:
- description: 'Pass your Darwin API key in the x-api-key header. You can also authenticate with Authorization: Bearer <apiKey>.'
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/darwin-so-openapi.json
  type: apiKey
- bearerFormat: Darwin API key or OAuth access token
  description: 'Pass a Darwin API key or OAuth access token as Authorization: Bearer <token>. You can also pass a Darwin API key in x-api-key.'
  name: bearer
  scheme: bearer
  sources:
  - openapi/darwin-so-openapi.json
  type: http
- description: The HTTP-only Darwin account session cookie set after sign-in. Local development uses better-auth.session_token without the __Secure- prefix.
  in: cookie
  name: AccountSession
  parameter: __Secure-better-auth.session_token
  sources:
  - openapi/darwin-so-openapi.json
  type: apiKey
slug: darwin-so-authentication
source_filename: darwin-so-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/darwin-so-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: 'Pass your Darwin API key in the x-api-key header. You can also authenticate\n    with Authorization: Bearer <apiKey>.'\n  sources:\n  - openapi/darwin-so-openapi.json\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: Darwin API key or OAuth access token\n  description: 'Pass a Darwin API key or OAuth access token as Authorization: Bearer <token>.\n    You can also pass a Darwin API key in x-api-key.'\n  sources:\n  - openapi/darwin-so-openapi.json\n- name: AccountSession\n  type: apiKey\n  in: cookie\n  parameter: __Secure-better-auth.session_token\n  description: The HTTP-only Darwin account session cookie set after sign-in. Local development\n    uses better-auth.session_token without the __Secure- prefix.\n\
  \  sources:\n  - openapi/darwin-so-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/darwin-so/authentication/darwin-so-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Artificial Intelligence
- Platform
- Developer Tools
- Marketplace
- Productivity
---
