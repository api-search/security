---
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Wallex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wallex secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Wallex
provider_slug: wallex
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter_name: X-Api-Key
  required: always
  source: docs
  type: apiKey
- bearer_format: opaque-token
  name: BearerAuth
  required: restricted-resources
  revocation: POST /v2/logout
  scheme: bearer
  source: docs
  token_endpoint: POST /v2/authenticate
  token_ttl_seconds: 28800
  type: http
slug: wallex-authentication
source_filename: wallex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.wallex.asia/docs/intro\ndocs:\n- https://docs.wallex.asia/docs/intro\n- https://docs.wallex.asia/docs/api/authentication/authenticate\n- https://docs.wallex.asia/docs/api/authentication/authenticate-yaml\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header]\n  model: >-\n    Two-layer auth. Every request carries a static X-Api-Key header for\n    identification. Restricted resources additionally require a short-lived\n    Bearer token (Authorization header) obtained by exchanging accessKeyId +\n    secretAccessKey at POST /v2/authenticate. Tokens are valid for 8 hours and\n    can be refreshed at any time; Log Out invalidates a token before expiry.\ncredentials:\n  provisioning: Credentials are issued by Wallex on request (contact@wallextech.com); there is no self-serve key page for the Partner API.\n  items:\n  - name: X-Api-Key\n    description: Static key that identifies the partner on every request. Missing/invalid\
  \ returns 403 Forbidden.\n  - name: accessKeyId\n    description: Used with secretAccessKey to obtain the authorization token.\n  - name: secretAccessKey\n    description: Used with accessKeyId to obtain the authorization token.\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: header\n    parameter_name: X-Api-Key\n    required: always\n    source: docs\n  - name: BearerAuth\n    type: http\n    scheme: bearer\n    bearer_format: opaque-token\n    token_endpoint: POST /v2/authenticate\n    token_ttl_seconds: 28800\n    required: restricted-resources\n    revocation: POST /v2/logout\n    source: docs\nmissing_header_behavior:\n  no_api_key: 403 Forbidden\n  no_authorization: 401 Unauthorized\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wallex/refs/heads/main/authentication/wallex-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Payments
- Cross-Border Payments
- Foreign Exchange
- Fintech
- Collections
- B2B Payments
- Embedded Finance
- Southeast Asia
---
