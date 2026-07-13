---
api_key_in: []
api_specs:
- filename: moov-api-openapi.yml
  format: yaml
  label: Moov API
  slug: moov-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/openapi/moov-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Moov Authentication
name_suffix: Authentication
oauth_flows: []
overview: Moov secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Moov
provider_slug: moov
scheme_count: 1
schemes:
- description: OAuth2 bearer token obtained from the /oauth2/token endpoint. Include in the Authorization header as "Bearer {token}".
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/moov-api-openapi.yml
  type: http
slug: moov-authentication
source_filename: moov-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/moov-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth2 bearer token obtained from the /oauth2/token endpoint. Include in the\n    Authorization header as \"Bearer {token}\".\n  sources:\n  - openapi/moov-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/authentication/moov-authentication.yml
summary_line: http · 1 scheme
tags:
- Banking
- Embedded Finance
- Financial Infrastructure
- Money Movement
- Payments
- Transfers
---
