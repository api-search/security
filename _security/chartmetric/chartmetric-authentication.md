---
api_key_in: []
api_specs:
- filename: chartmetric-openapi.yml
  format: yaml
  label: Chartmetric Artists API
  slug: artists
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chartmetric/refs/heads/main/openapi/chartmetric-openapi.yml
- filename: chartmetric-openapi.yml
  format: yaml
  label: Chartmetric Tracks API
  slug: tracks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chartmetric/refs/heads/main/openapi/chartmetric-openapi.yml
- filename: chartmetric-openapi.yml
  format: yaml
  label: Chartmetric Albums API
  slug: albums
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chartmetric/refs/heads/main/openapi/chartmetric-openapi.yml
- filename: chartmetric-openapi.yml
  format: yaml
  label: Chartmetric Playlists API
  slug: playlists
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chartmetric/refs/heads/main/openapi/chartmetric-openapi.yml
- filename: chartmetric-openapi.yml
  format: yaml
  label: Chartmetric Charts API
  slug: charts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chartmetric/refs/heads/main/openapi/chartmetric-openapi.yml
- filename: chartmetric-openapi.yml
  format: yaml
  label: Chartmetric Stats and Metrics API
  slug: stats-metrics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chartmetric/refs/heads/main/openapi/chartmetric-openapi.yml
- filename: chartmetric-openapi.yml
  format: yaml
  label: Chartmetric Search API
  slug: search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chartmetric/refs/heads/main/openapi/chartmetric-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Chartmetric Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chartmetric secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Chartmetric
provider_slug: chartmetric
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer access token obtained from POST /token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/chartmetric-openapi.yml
  type: http
slug: chartmetric-authentication
source_filename: chartmetric-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/chartmetric-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer access token obtained from POST /token.\n  sources:\n  - openapi/chartmetric-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chartmetric/refs/heads/main/authentication/chartmetric-authentication.yml
summary_line: http · 1 scheme
tags:
- Music
- Analytics
- Artist Intelligence
- Streaming
- Charts
---
