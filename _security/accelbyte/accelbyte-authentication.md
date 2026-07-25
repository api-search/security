---
api_key_in: []
api_specs:
- filename: accelbyte-achievement-api-openapi.yml
  format: yaml
  label: AccelByte Achievement API
  slug: accelbyte-achievement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-achievement-api-openapi.yml
- filename: accelbyte-basic-api-openapi.yml
  format: yaml
  label: AccelByte Basic API
  slug: accelbyte-basic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-basic-api-openapi.yml
- filename: accelbyte-cloud-save-api-openapi.yml
  format: yaml
  label: AccelByte Cloud Save API
  slug: accelbyte-cloud-save-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-cloud-save-api-openapi.yml
- filename: accelbyte-dsmc-api-openapi.yml
  format: yaml
  label: AccelByte DSMC API
  slug: accelbyte-dsmc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-dsmc-api-openapi.yml
- filename: accelbyte-game-telemetry-api-openapi.yml
  format: yaml
  label: AccelByte Game Telemetry API
  slug: accelbyte-game-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-game-telemetry-api-openapi.yml
- filename: accelbyte-iam-api-openapi.yml
  format: yaml
  label: AccelByte IAM API
  slug: accelbyte-iam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-iam-api-openapi.yml
- filename: accelbyte-leaderboard-api-openapi.yml
  format: yaml
  label: AccelByte Leaderboard API
  slug: accelbyte-leaderboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-leaderboard-api-openapi.yml
- filename: accelbyte-matchmaking-api-openapi.yml
  format: yaml
  label: AccelByte Matchmaking API
  slug: accelbyte-matchmaking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-matchmaking-api-openapi.yml
- filename: accelbyte-platform-api-openapi.yml
  format: yaml
  label: AccelByte Platform API
  slug: accelbyte-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-platform-api-openapi.yml
- filename: accelbyte-season-pass-api-openapi.yml
  format: yaml
  label: AccelByte Season Pass API
  slug: accelbyte-season-pass-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-season-pass-api-openapi.yml
- filename: accelbyte-session-api-openapi.yml
  format: yaml
  label: AccelByte Session API
  slug: accelbyte-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-session-api-openapi.yml
- filename: accelbyte-statistics-api-openapi.yml
  format: yaml
  label: AccelByte Statistics API
  slug: accelbyte-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-statistics-api-openapi.yml
- filename: accelbyte-ugc-api-openapi.yml
  format: yaml
  label: AccelByte UGC API
  slug: accelbyte-ugc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-ugc-api-openapi.yml
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
