---
api_key_in: []
api_specs:
- filename: palla-platform-openapi.yml
  format: yaml
  label: Palla Platform Partner API
  slug: palla-platform-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/palla/refs/heads/main/openapi/palla-platform-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Palla Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Palla secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Palla
provider_slug: palla
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Partner Bearer token obtained from POST /v1/auth/token via a client_credentials exchange. Scoped to a single User via user_id.
  name: partnerToken
  scheme: bearer
  sources:
  - openapi/palla-platform-openapi.yml
  type: http
- description: Partner credential exchange (client_credentials grant). Sent as a JSON body to /v1/auth/token with client_id, client_secret, audience, and user_id; returns a Bearer token in data.token.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.platform.palla.app/v1/auth/token
  name: clientCredentials
  sources:
  - openapi/palla-platform-openapi.yml
  type: oauth2
slug: palla-authentication
source_filename: palla-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/palla-platform-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: partnerToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Partner Bearer token obtained from POST /v1/auth/token via a client_credentials\n    exchange. Scoped to a single User via user_id.\n  sources:\n  - openapi/palla-platform-openapi.yml\n- name: clientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.platform.palla.app/v1/auth/token\n    scopes: 0\n  description: Partner credential exchange (client_credentials grant). Sent as a JSON body to\n    /v1/auth/token with client_id, client_secret, audience, and user_id; returns a Bearer token\n    in data.token.\n  sources:\n  - openapi/palla-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/palla/refs/heads/main/authentication/palla-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Fintech
- Payments
- Cross-Border Payments
- Remittances
- P2P Payments
- Money Transfer
- Embedded Finance
---
