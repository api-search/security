---
api_key_in: []
api_specs:
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte IAM API
  slug: accelbyte-iam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte Basic (Player Profile) API
  slug: accelbyte-basic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte Cloud Save API
  slug: accelbyte-cloudsave-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte Statistics & Leaderboard API
  slug: accelbyte-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte Matchmaking API
  slug: accelbyte-matchmaking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte Lobby & Session API
  slug: accelbyte-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte Commerce (Platform) API
  slug: accelbyte-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte Seasons & Battle Pass API
  slug: accelbyte-seasonpass-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte Achievement API
  slug: accelbyte-achievement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte Dedicated Server (Armada/DSMC) API
  slug: accelbyte-dsmc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte Analytics & Telemetry API
  slug: accelbyte-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte UGC API
  slug: accelbyte-ugc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Accelbyte Authentication
name_suffix: Authentication
oauth_flows: []
overview: AccelByte secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AccelByte
provider_slug: accelbyte
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: OAuth2 access token issued by the IAM token endpoint.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/accelbyte-openapi.yml
  type: http
- description: OAuth2 client id / client secret used at the token endpoint.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/accelbyte-openapi.yml
  type: http
slug: accelbyte-authentication
source_filename: accelbyte-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/accelbyte-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth2 access token issued by the IAM token endpoint.\n  sources:\n  - openapi/accelbyte-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: OAuth2 client id / client secret used at the token endpoint.\n  sources:\n  - openapi/accelbyte-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/authentication/accelbyte-authentication.yml
summary_line: http · 2 schemes
tags:
- Gaming
- Backend
- BaaS
- Live Services
- Player Accounts
- Commerce
---
