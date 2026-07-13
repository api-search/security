---
api_key_in: []
api_specs:
- filename: nimble-openapi.yml
  format: yaml
  label: Nimble REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Nimble Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Nimble secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Nimble
provider_slug: nimble
scheme_count: 1
schemes:
- description: 'OAuth 2.0 bearer token. Provide the token via either the

    `Authorization: Bearer <token>` header or the

    `access_token=<token>` query parameter.'
  flows:
  - authorizationUrl: https://app.nimble.com/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://app.nimble.com/oauth/token
  name: bearerAuth
  sources:
  - openapi/nimble-openapi.yml
  type: oauth2
slug: nimble-authentication
source_filename: nimble-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nimble-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.nimble.com/oauth/authorize\n    tokenUrl: https://app.nimble.com/oauth/token\n    scopes: 0\n  description: |-\n    OAuth 2.0 bearer token. Provide the token via either the\n    `Authorization: Bearer <token>` header or the\n    `access_token=<token>` query parameter.\n  sources:\n  - openapi/nimble-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/authentication/nimble-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- CRM
- Sales
- Contact Management
- Relationship Management
- Marketing Automation
- Pipeline Management
---
