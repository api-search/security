---
api_key_in:
- header
api_specs:
- filename: planetscale-platform-api-openapi.yml
  format: yaml
  label: PlanetScale Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planetscale/refs/heads/main/openapi/planetscale-platform-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Planetscale Authentication
name_suffix: Authentication
oauth_flows: []
overview: planetscale secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: planetscale
provider_slug: planetscale
scheme_count: 2
schemes:
- description: Service token authentication. Use the format 'ServiceToken {token_id}:{token_value}' in the Authorization header.
  in: header
  name: serviceToken
  parameter: Authorization
  sources:
  - openapi/planetscale-platform-api-openapi.yml
  type: apiKey
- description: OAuth 2.0 bearer token authentication. Obtain tokens via the PlanetScale OAuth authorization code flow.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/planetscale-platform-api-openapi.yml
  type: http
slug: planetscale-authentication
source_filename: planetscale-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/planetscale-platform-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: serviceToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Service token authentication. Use the format 'ServiceToken {token_id}:{token_value}'\n    in the Authorization header.\n  sources:\n  - openapi/planetscale-platform-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 bearer token authentication. Obtain tokens via the PlanetScale OAuth\n    authorization code flow.\n  sources:\n  - openapi/planetscale-platform-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/planetscale/refs/heads/main/authentication/planetscale-authentication.yml
summary_line: apiKey/http · 2 schemes
tags: []
---
