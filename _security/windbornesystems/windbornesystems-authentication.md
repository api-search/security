---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Windbornesystems Authentication
name_suffix: Authentication
oauth_flows: []
overview: WindBorne Systems declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: WindBorne Systems
provider_slug: windbornesystems
scheme_count: 2
schemes:
- description: Primary authentication - pass your WindBorne API key as a Bearer token. Keys are issued from the developer portal.
  env:
  - WB_API_KEY
  - WB_CLIENT_ID
  format: 'Authorization: Bearer $WB_API_KEY'
  header: Authorization
  id: api_key_bearer
  in: header
  key_management: https://app.windbornesystems.com/api_tokens
  scheme: bearer
  type: http
- algorithm: HS256
  bearer_format: JWT
  description: 'Optional signed-JWT flow for browser/untrusted runtimes. Generate a signed JWT with payload {"iat": CURRENT_UNIX_TIMESTAMP} using HS256 and your WB_API_KEY as the secret, then send it as Authorization Bearer - avoids exposing the raw API key to the caller.'
  id: jwt_hs256
  scheme: bearer
  type: http
slug: windbornesystems-authentication
source_filename: windbornesystems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: api.windbornesystems.com/getting-started + /technical-guides/authentication/jwt-tokens\ndocs: https://api.windbornesystems.com/technical-guides/authentication/jwt-tokens\napi: WindBorne Data API\nbase_url: https://api.windbornesystems.com\nschemes:\n- id: api_key_bearer\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer $WB_API_KEY'\n  description: Primary authentication - pass your WindBorne API key as a Bearer token.\n    Keys are issued from the developer portal.\n  key_management: https://app.windbornesystems.com/api_tokens\n  env:\n  - WB_API_KEY\n  - WB_CLIENT_ID\n- id: jwt_hs256\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  algorithm: HS256\n  description: 'Optional signed-JWT flow for browser/untrusted runtimes. Generate a\n    signed JWT with payload {\"iat\": CURRENT_UNIX_TIMESTAMP} using HS256 and your WB_API_KEY\n    as the secret, then send it as\
  \ Authorization Bearer - avoids exposing the raw\n    API key to the caller.'\noauth2: false\nopenid_connect: false\nmutual_tls: false\nnotes: No OAuth2/OIDC authorization server or .well-known metadata is published; auth\n  is a static per-account API key optionally wrapped in an HS256-signed JWT.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/windbornesystems/refs/heads/main/authentication/windbornesystems-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Weather
- Weather Data
- Forecasting
- Atmospheric Data
- Geospatial
- Climate
- Machine Learning
- MCP
---
