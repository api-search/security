---
api_key_in: []
api_specs:
- filename: rubrik-client-token-api-openapi.yml
  format: yaml
  label: Rubrik Client Token API
  slug: rubrik-client-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubrik/refs/heads/main/openapi/rubrik-client-token-api-openapi.yml
- filename: rubrik-graphql-api-openapi.yml
  format: yaml
  label: Rubrik Graphql API
  slug: rubrik-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubrik/refs/heads/main/openapi/rubrik-graphql-api-openapi.yml
- filename: rubrik-oauth-api-openapi.yml
  format: yaml
  label: Rubrik Oauth API
  slug: rubrik-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubrik/refs/heads/main/openapi/rubrik-oauth-api-openapi.yml
- filename: rubrik-session-api-openapi.yml
  format: yaml
  label: Rubrik Session API
  slug: rubrik-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubrik/refs/heads/main/openapi/rubrik-session-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Rubrik Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rubrik secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rubrik
provider_slug: rubrik
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth2 access token obtained via /client_token or /oauth/token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/rubrik-openapi.yml
  type: http
slug: rubrik-authentication
source_filename: rubrik-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rubrik-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth2 access token obtained via /client_token or /oauth/token.\n  sources:\n  - openapi/rubrik-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rubrik/refs/heads/main/authentication/rubrik-authentication.yml
summary_line: http · 1 scheme
tags:
- Backup
- Cyber Recovery
- Data Security
- Data Security Posture Management
- GraphQL
- Ransomware Recovery
- REST API
- SaaS Protection
- Threat Analytics
- Zero Trust
---
