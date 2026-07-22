---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Silvercar Authentication
name_suffix: Authentication
oauth_flows: []
overview: silvercar declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: silvercar
provider_slug: silvercar
scheme_count: 2
schemes:
- authorization_server: https://dealerware.auth0.com/
  description: Machine-to-machine (M2M) authentication. Partners exchange a Client ID and Client Secret (issued by Dealerware, requested via partnersupport@dealerware.com) at the Auth0 authorization server for a short-lived, RS256-signed JWT access token. Subsequent Dealerware API calls send only the access token.
  flow: clientCredentials
  grant_type: client_credentials
  identity_provider: Auth0
  jwks_uri: https://dealerware.auth0.com/.well-known/jwks.json
  token_endpoint: https://dealerware.auth0.com/oauth/token
  token_format: JWT
  token_signing_alg: RS256
  type: oauth2
- bearer_format: JWT
  description: All Dealerware API requests carry the access token as a Bearer token in the Authorization header. HTTPS is required for every request. Requests missing or presenting an invalid token are rejected with an authentication error.
  header: Authorization
  in: header
  scheme: bearer
  type: http
slug: silvercar-authentication
source_filename: silvercar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.dealerware.com/docs/api-integration-process.md\nname: Dealerware Partner Integration API — Authentication Profile\nnote: >-\n  Silvercar's technology and developer surface now operate as Dealerware;\n  silvercar.com issues a 301 redirect to dealerware.com. The public API and its\n  authentication are documented at developer.dealerware.com.\nschemes:\n- type: oauth2\n  flow: clientCredentials\n  grant_type: client_credentials\n  description: >-\n    Machine-to-machine (M2M) authentication. Partners exchange a Client ID and\n    Client Secret (issued by Dealerware, requested via partnersupport@dealerware.com)\n    at the Auth0 authorization server for a short-lived, RS256-signed JWT access\n    token. Subsequent Dealerware API calls send only the access token.\n  authorization_server: https://dealerware.auth0.com/\n  token_endpoint: https://dealerware.auth0.com/oauth/token\n  jwks_uri: https://dealerware.auth0.com/.well-known/jwks.json\n\
  \  token_format: JWT\n  token_signing_alg: RS256\n  identity_provider: Auth0\n- type: http\n  scheme: bearer\n  bearer_format: JWT\n  description: >-\n    All Dealerware API requests carry the access token as a Bearer token in the\n    Authorization header. HTTPS is required for every request. Requests missing\n    or presenting an invalid token are rejected with an authentication error.\n  in: header\n  header: Authorization\ncredential_issuance: manual\ncredential_contact: partnersupport@dealerware.com\napi_host: https://api.dealerware.com\ndocs:\n- https://developer.dealerware.com/docs/api-integration-process.md\n- https://developer.dealerware.com/recipes/dealerware-api-authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/silvercar/refs/heads/main/authentication/silvercar-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Automotive
- Car Rental
- Fleet Management
- Mobility
- Dealership
- Rental
- SaaS
---
