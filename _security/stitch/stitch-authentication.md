---
api_key_in: []
api_specs:
- filename: stitch-openapi.yml
  format: yaml
  label: Stitch GraphQL API
  slug: stitch-graphql
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stitch/refs/heads/main/openapi/stitch-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Stitch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stitch secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Stitch
provider_slug: stitch
scheme_count: 1
schemes:
- description: OAuth 2.0 Bearer token from the Stitch identity server.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/stitch-openapi.yml
  type: http
slug: stitch-authentication
source_filename: stitch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stitch-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 Bearer token from the Stitch identity server.\n  sources:\n  - openapi/stitch-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stitch/refs/heads/main/authentication/stitch-authentication.yml
summary_line: http · 1 scheme
tags:
- Africa
- Financial Data
- Open Banking
- Payments
- Unified API
- South Africa
- Nigeria
---
