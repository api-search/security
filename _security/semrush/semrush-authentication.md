---
api_key_in: []
api_specs:
- filename: semrush-openapi.yml
  format: yaml
  label: Semrush
  slug: semrush
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semrush/refs/heads/main/openapi/semrush-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Semrush Authentication
name_suffix: Authentication
oauth_flows: []
overview: Semrush secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Semrush
provider_slug: semrush
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Use token retrieved from Jwt Issuer

    [Documentation](https://www.semrush.com/apps/docs/server-to-server-api/bearer-token)'
  name: jwtIssuerToken
  scheme: bearer
  sources:
  - openapi/semrush-openapi.yml
  type: http
slug: semrush-authentication
source_filename: semrush-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/semrush-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: jwtIssuerToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    Use token retrieved from Jwt Issuer\n    [Documentation](https://www.semrush.com/apps/docs/server-to-server-api/bearer-token)\n  sources:\n  - openapi/semrush-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/semrush/refs/heads/main/authentication/semrush-authentication.yml
summary_line: http · 1 scheme
tags:
- Data
- Search Engines
---
