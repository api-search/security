---
api_key_in: []
api_specs:
- filename: medium-rest-api-openapi.yml
  format: yaml
  label: Medium REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medium/refs/heads/main/openapi/medium-rest-api-openapi.yml
- filename: medium-oauth2-openapi.yml
  format: yaml
  label: Medium OAuth2 API
  slug: oauth2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medium/refs/heads/main/openapi/medium-oauth2-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Medium Authentication
name_suffix: Authentication
oauth_flows: []
overview: medium secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: medium
provider_slug: medium
scheme_count: 1
schemes:
- description: Self-issued access token generated from Medium account settings or an OAuth2 access token obtained via the authorization flow.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/medium-rest-api-openapi.yml
  type: http
slug: medium-authentication
source_filename: medium-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/medium-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Self-issued access token generated from Medium account settings or an OAuth2\n    access token obtained via the authorization flow.\n  sources:\n  - openapi/medium-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medium/refs/heads/main/authentication/medium-authentication.yml
summary_line: http · 1 scheme
tags: []
---
