---
api_key_in: []
api_specs:
- filename: phasio-openapi-original.json
  format: json
  label: Phasio Manufacturer API
  slug: phasio-manufacturer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phasio/refs/heads/main/openapi/phasio-openapi-original.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Phasio Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Phasio secures its APIs with http and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Phasio
provider_slug: phasio
scheme_count: 1
schemes:
- bearerFormat: JWT
  in: header
  name: Phasio API Bearer Token
  note: Access token obtained via OAuth 2.0 client-credentials, sent as Bearer JWT.
  parameter: Authorization
  scheme: bearer
  sources:
  - openapi/phasio-openapi-original.json
  type: http
slug: phasio-authentication
source_filename: phasio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/phasio-openapi-original.json\ndocs: https://docs.phas.io/developers\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\noauth2:\n  grant: client_credentials\n  token_endpoint: https://auth.eu.phas.io/oauth2/token\n  issuer: https://auth.eu.phas.io\n  oidc_discovery: https://auth.eu.phas.io/.well-known/openid-configuration\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - tls_client_auth\n  credentials_note: client_id/client_secret generated under Settings > API Keys in the manufacturer dashboard.\nschemes:\n- name: Phasio API Bearer Token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  in: header\n  parameter: Authorization\n  note: Access token obtained via OAuth 2.0 client-credentials, sent as Bearer JWT.\n  sources:\n  - openapi/phasio-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phasio/refs/heads/main/authentication/phasio-authentication.yml
summary_line: http/oauth2 · 1 scheme
tags:
- Company
- Manufacturing
- Additive Manufacturing
- 3D Printing
- CNC Machining
- Quoting
- Production Operations
- Manufacturing Execution
- API
---
