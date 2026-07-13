---
api_key_in:
- query
api_specs:
- filename: ghost-admin-api-openapi.yml
  format: yaml
  label: Ghost Admin API
  slug: ghost-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/openapi/ghost-admin-api-openapi.yml
- filename: ghost-content-api-openapi.yml
  format: yaml
  label: Ghost Content API
  slug: ghost-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/openapi/ghost-content-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ghost Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ghost secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ghost
provider_slug: ghost
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: JSON Web Token generated from an Admin API key. The key is split into an ID and secret at the colon separator. The ID is used as the kid header and the secret is used to sign the token with HS256.
  name: adminApiToken
  scheme: bearer
  sources:
  - openapi/ghost-admin-api-openapi.yml
  type: http
- description: Content API key obtained from a custom integration in Ghost Admin. Content API keys are safe for use in browsers and other insecure environments as they only provide access to public data.
  in: query
  name: contentApiKey
  parameter: key
  sources:
  - openapi/ghost-content-api-openapi.yml
  type: apiKey
slug: ghost-authentication
source_filename: ghost-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ghost-admin-api-openapi.yml, openapi/ghost-content-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: adminApiToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JSON Web Token generated from an Admin API key. The key is split into an ID and\n    secret at the colon separator. The ID is used as the kid header and the secret is used to\n    sign the token with HS256.\n  sources:\n  - openapi/ghost-admin-api-openapi.yml\n- name: contentApiKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: Content API key obtained from a custom integration in Ghost Admin. Content API\n    keys are safe for use in browsers and other insecure environments as they only provide access\n    to public data.\n  sources:\n  - openapi/ghost-content-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/authentication/ghost-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Publishing
- Newsletters
- Memberships
- Content
- Open Source
---
