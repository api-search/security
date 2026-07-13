---
api_key_in:
- query
api_specs:
- filename: matomo-openapi.yml
  format: yaml
  label: Matomo Reporting API
  slug: reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matomo/refs/heads/main/openapi/matomo-openapi.yml
- filename: matomo-tracking-openapi.yml
  format: yaml
  label: Matomo Tracking API
  slug: tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matomo/refs/heads/main/openapi/matomo-tracking-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Matomo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Matomo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Matomo
provider_slug: matomo
scheme_count: 1
schemes:
- description: 'Matomo auth token created in Administration > Personal > Security >

    Auth tokens. May be passed as a query parameter or, preferably, in

    the POST body.'
  in: query
  name: TokenAuth
  parameter: token_auth
  sources:
  - openapi/matomo-openapi.yml
  - openapi/matomo-tracking-openapi.yml
  type: apiKey
slug: matomo-authentication
source_filename: matomo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/matomo-openapi.yml, openapi/matomo-tracking-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: query\n  parameter: token_auth\n  description: |-\n    Matomo auth token created in Administration > Personal > Security >\n    Auth tokens. May be passed as a query parameter or, preferably, in\n    the POST body.\n  sources:\n  - openapi/matomo-openapi.yml\n  - openapi/matomo-tracking-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matomo/refs/heads/main/authentication/matomo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Analytics
- Data Ownership
- Open Source
- Privacy
- Self-Hosted
- Web Analytics
---
