---
api_key_in:
- header
api_specs:
- filename: genesys-platform-api-openapi-original.json
  format: json
  label: Genesys Cloud Platform API
  slug: genesys-cloud-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genesys/refs/heads/main/openapi/genesys-platform-api-openapi-original.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Genesys Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Genesys secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Genesys
provider_slug: genesys
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://login.mypurecloud.com/authorize
    flow: implicit
    scopes: 1
  name: PureCloud OAuth
  sources:
  - openapi/genesys-platform-api-openapi-original.json
  type: oauth2
- in: header
  name: Guest Chat JWT
  parameter: Authorization
  sources:
  - openapi/genesys-platform-api-openapi-original.json
  type: apiKey
slug: genesys-authentication
source_filename: genesys-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/genesys-platform-api-openapi-original.json\ndocs: https://developer.genesys.cloud/authorization/platform-auth/\nauthorization_server: https://login.mypurecloud.com\nwell_known: well-known/genesys-oauth-authorization-server.json\ngrant_types_supported:\n- authorization_code\n- client_credentials\n- refresh_token\n- urn:ietf:params:oauth:grant-type:saml2-bearer\n- implicit\npkce: S256\ntoken_endpoint: https://login.mypurecloud.com/oauth/token\nauthorization_endpoint: https://login.mypurecloud.com/oauth/authorize\nnotes: >-\n  The OpenAPI declares only the implicit flow, but the published OAuth 2.0\n  authorization-server metadata at login.mypurecloud.com advertises\n  authorization_code (with PKCE S256), client_credentials, refresh_token, and\n  SAML2 bearer grants. Scope enforcement is opt-in per organization.\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - implicit\nschemes:\n\
  - name: PureCloud OAuth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.mypurecloud.com/authorize\n    scopes: 1\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- name: Guest Chat JWT\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genesys/refs/heads/main/authentication/genesys-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Software
- Contact Center
- Customer Experience
- CCaaS
- Telephony
- Conversational AI
- Workforce Management
- Cloud Communications
- CPaaS
---
