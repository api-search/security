---
api_key_in: []
api_specs:
- filename: door-partner-openapi.json
  format: json
  label: OpenDOOR Partner API
  slug: opendoor-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/door/refs/heads/main/openapi/door-partner-openapi.json
- filename: door-authentication-openapi.json
  format: json
  label: OpenDOOR Authentication API
  slug: opendoor-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/door/refs/heads/main/openapi/door-authentication-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Door Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- passwordless
overview: Door secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and passwordless flow(s).
provider_name: Door
provider_slug: door
scheme_count: 3
schemes:
- applies_to: openapi/door-partner-openapi.json
  bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/door-partner-openapi.json
  type: http
- description: Partner-scoped (machine-to-machine) token for non-user OpenDOOR API calls. Client ID/Secret provisioned by DOOR through secure channels; DOOR reserves the right to rotate the secret.
  flow: clientCredentials
  name: partner-m2m
  sources:
  - https://developers.door.com/docs/partner-backend.md
  - openapi/door-authentication-openapi.json
  token_url: https://auth.prod.latch.com/oauth/token
  type: oauth2
- description: User-scoped token obtained via email-based verification code (Auth0 passwordless, connection=email). Used to make SDK/API calls on behalf of a provisioned end-user. No user password is collected.
  flow: passwordless
  name: user-passwordless
  sources:
  - https://developers.door.com/docs/partner-backend.md
  - openapi/door-authentication-openapi.json
  start_url: https://auth.prod.latch.com/passwordless/start
  token_url: https://auth.prod.latch.com/oauth/token
  type: oauth2
slug: door-authentication
source_filename: door-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/door-partner-openapi.json, openapi/door-authentication-openapi.json\ndocs: https://developers.door.com/docs/partner-backend.md\nsummary:\n  types:\n  - http\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - clientCredentials\n  - passwordless\nmodel: >-\n  OpenDOOR uses Auth0 (auth.prod.latch.com) as its identity provider. DOOR issues each\n  partner a unique Auth0 application with two credential sets: partner-scoped (machine-to-machine,\n  client_credentials) and user-scoped (passwordless, email verification code). The Partner\n  backend exchanges its Client ID/Secret for a JWT; the JWT is presented as a Bearer token\n  to the OpenDOOR Partner REST API (rest.latchaccess.com). Tokens are scoped by claims\n  (Partner ID, and User ID for user-scoped tokens) rather than by OAuth scope strings.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applies_to: openapi/door-partner-openapi.json\n\
  \  sources:\n  - openapi/door-partner-openapi.json\n- name: partner-m2m\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://auth.prod.latch.com/oauth/token\n  description: >-\n    Partner-scoped (machine-to-machine) token for non-user OpenDOOR API calls. Client ID/Secret\n    provisioned by DOOR through secure channels; DOOR reserves the right to rotate the secret.\n  sources:\n  - https://developers.door.com/docs/partner-backend.md\n  - openapi/door-authentication-openapi.json\n- name: user-passwordless\n  type: oauth2\n  flow: passwordless\n  start_url: https://auth.prod.latch.com/passwordless/start\n  token_url: https://auth.prod.latch.com/oauth/token\n  description: >-\n    User-scoped token obtained via email-based verification code (Auth0 passwordless, connection=email).\n    Used to make SDK/API calls on behalf of a provisioned end-user. No user password is collected.\n  sources:\n  - https://developers.door.com/docs/partner-backend.md\n  - openapi/door-authentication-openapi.json\n\
  idp:\n  provider: Auth0\n  issuer: https://auth.prod.latch.com/\n  openid_configuration: well-known/door-openid-configuration.json\n  jwks_uri: https://auth.prod.latch.com/.well-known/jwks.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/door/refs/heads/main/authentication/door-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Access Control
- Smart Building
- Proptech
- Physical Security
- IoT
- Multifamily
- Real Estate
- Smart Lock
- Building Automation
---
