---
api_key_in: []
api_specs:
- filename: volteras-connect-openapi-original.json
  format: json
  label: Volteras Connect API
  slug: volteras-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/volteras/refs/heads/main/openapi/volteras-connect-openapi-original.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Volteras Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Volteras secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Volteras
provider_slug: volteras
scheme_count: 2
schemes:
- name: HTTPBasic
  scheme: basic
  sources:
  - openapi/volteras-connect-openapi-original.json
  type: http
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: /v1/oauth2/token
  name: OAuth2ClientCredentialsBearer
  sources:
  - openapi/volteras-connect-openapi-original.json
  type: oauth2
slug: volteras-authentication
source_filename: volteras-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/volteras-connect-openapi-original.json\ndocs: https://docs.volteras.com/api-reference/authentication/auth-token\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  notes: >-\n    Volteras Connect adheres to OAuth 2.0: applications created in the Volteras\n    Portal (per environment, sandbox vs production) issue a client_id /\n    client_secret, exchanged at POST /v1/oauth2/token for access + refresh\n    tokens; requests carry Authorization: Bearer <access-token>. POST\n    /v1/oauth2/test-token validates a token and returns the associated clientId\n    and organizationId. The HTTPBasic scheme in the spec covers client\n    authentication on the token endpoint. End-user data access is governed\n    separately by consent scopes (see scopes/volteras-scopes.yml).\nendpoints:\n  token: /v1/oauth2/token\n  test_token: /v1/oauth2/test-token\n  sandbox_token_test: https://api.sandbox.volteras.com/v1/oauth2/test-token\n\
  credentials:\n  issuer: https://portal.volteras.com/ (Applications section, one application per environment)\nschemes:\n- name: HTTPBasic\n  type: http\n  scheme: basic\n  sources:\n  - openapi/volteras-connect-openapi-original.json\n- name: OAuth2ClientCredentialsBearer\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/oauth2/token\n    scopes: 0\n  sources:\n  - openapi/volteras-connect-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/volteras/refs/heads/main/authentication/volteras-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Electric Vehicles
- Connected Vehicles
- Automotive
- Vehicle Telemetry
- EV Charging
- Energy
- Mobility
- Fleet Management
---
