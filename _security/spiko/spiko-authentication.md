---
api_key_in: []
api_specs:
- filename: spiko-public-openapi.json
  format: json
  label: Spiko Public API
  slug: spiko-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spiko/refs/heads/main/openapi/spiko-public-openapi.json
- filename: spiko-investor-openapi.json
  format: json
  label: Spiko Investor API
  slug: spiko-investor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spiko/refs/heads/main/openapi/spiko-investor-openapi.json
- filename: spiko-distributor-openapi.json
  format: json
  label: Spiko Distributor API
  slug: spiko-distributor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spiko/refs/heads/main/openapi/spiko-distributor-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Spiko Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Spiko secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Spiko
provider_slug: spiko
scheme_count: 2
schemes:
- description: HTTP Basic authentication using your API client_id as the username and client_secret as the password. Primary mechanism for the Distributor API and an option for the Investor API. Both methods grant full access to all endpoints.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/spiko-distributor-openapi.json
  - openapi/spiko-investor-openapi.json
  type: http
  used_by:
  - Investor API
  - Distributor API
- description: OAuth 2.0 authorization code flow with PKCE (S256) for the Investor API, issuing revocable, scoped Bearer tokens. Authorization server publishes an OpenID Connect discovery document. Token endpoint auth methods include client_secret_basic, client_secret_post, private_key_jwt, and none.
  flows:
  - authorizationUrl: https://investor-auth.spiko.io/oauth2/auth
    code_challenge_methods:
    - S256
    - plain
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://investor-auth.spiko.io/oauth2/token
    well_known: https://investor-auth.spiko.io/.well-known/openid-configuration
  name: oauth2
  sources:
  - openapi/spiko-investor-openapi.json
  type: oauth2
  used_by:
  - Investor API
slug: spiko-authentication
source_filename: spiko-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/spiko-distributor-openapi.json, openapi/spiko-investor-openapi.json\ndocs:\n- https://docs.spiko.io/developers/investor_api/getting_started\n- https://docs.spiko.io/developers/distributor_api/getting_started\n- https://docs.spiko.io/developers/public_api/getting_started\nsummary:\n  types:\n  - http\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  by_api:\n    public: none (open, no authentication)\n    investor: HTTP Basic (client_id/client_secret) OR OAuth 2.0 authorization code\n    distributor: HTTP Basic (client_id/client_secret)\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic authentication using your API client_id as the username and\n    client_secret as the password. Primary mechanism for the Distributor API and\n    an option for the Investor API. Both methods grant full access to all\n    endpoints.\n  used_by:\n  - Investor API\n  - Distributor\
  \ API\n  sources:\n  - openapi/spiko-distributor-openapi.json\n  - openapi/spiko-investor-openapi.json\n- name: oauth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 authorization code flow with PKCE (S256) for the Investor API,\n    issuing revocable, scoped Bearer tokens. Authorization server publishes an\n    OpenID Connect discovery document. Token endpoint auth methods include\n    client_secret_basic, client_secret_post, private_key_jwt, and none.\n  used_by:\n  - Investor API\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://investor-auth.spiko.io/oauth2/auth\n    tokenUrl: https://investor-auth.spiko.io/oauth2/token\n    well_known: https://investor-auth.spiko.io/.well-known/openid-configuration\n    code_challenge_methods:\n    - S256\n    - plain\n    scopes: 3\n  sources:\n  - openapi/spiko-investor-openapi.json\nnotes: >-\n  The Public API requires no authentication. The Distributor API additionally\n  mints short-lived investor JWTs (investorTokens.createInvestorToken)\
  \ so a\n  distributor can act on behalf of an onboarded investor; see the investor_jwt\n  technical guide.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spiko/refs/heads/main/authentication/spiko-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Fintech
- Money Market Funds
- Treasury Management
- Tokenization
- Cash Management
- Payments
- Webhooks
---
