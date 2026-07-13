---
api_key_in: []
api_specs:
- filename: trakt-openapi.yml
  format: yaml
  label: Trakt API v2
  slug: trakt-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trakt/refs/heads/main/openapi/trakt-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Trakt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trakt secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Trakt
provider_slug: trakt
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 access token from /oauth/token or /oauth/device/token. Send via Authorization header and required headers trakt-api-version (2) and trakt-api-key (client_id).
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/trakt-openapi.yml
  type: http
slug: trakt-authentication
source_filename: trakt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/trakt-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 access token from /oauth/token or /oauth/device/token. Send via Authorization\n    header and required headers trakt-api-version (2) and trakt-api-key (client_id).\n  sources:\n  - openapi/trakt-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trakt/refs/heads/main/authentication/trakt-authentication.yml
summary_line: http · 1 scheme
tags:
- Video
- Movies
- Television
- Media Tracking
- Scrobble
- Recommendations
- Social
- OAuth2
- Public APIs
---
