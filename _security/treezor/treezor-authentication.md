---
anonymous_access: false
api_key_in: []
api_specs:
- filename: treezor-openapi-generated.yml
  format: yaml
  label: Treezor API
  slug: treezor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treezor/refs/heads/main/openapi/_ae-authored/treezor-openapi-generated.yml
auth_types: []
description: Treezor uses OAuth2 with JWT tokens and Mutual TLS as an additional security layer.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Treezor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Treezor declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Treezor
provider_slug: treezor
scheme_count: 2
schemes:
- evidence: Treezor leverages the OAuth2 framework and JSON Web Token (JWT) which allows for a wide range of authentication flows.
  flows:
  - client_credentials
  - authorization_code
  how_to_obtain: Call the /oauth/token endpoint with client_id and client_secret (client_credentials) or exchange an authorization code (authorization_code) to receive a JWT.
  name: OAuth2
  scopes:
  - read_only
  - read_write
  - admin
  - keys
  - legal
  token_url: /oauth/token
  type: oauth2
- evidence: Treezor also relies on Mutual TLS authentication as an additional security layer.
  how_to_obtain: Mutual TLS is configured per environment; credentials are provided by Treezor Account Manager.
  name: Mutual TLS
  type: mtls
slug: treezor-authentication
source_filename: treezor-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.treezor.com/guide/api-basics/authentication.html
source_yaml: "generated: '2026-10-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.treezor.com/guide/api-basics/authentication.html\nsources:\n- https://docs.treezor.com/guide/api-basics/authentication.html\n- https://docs.treezor.com/guide/api-basics/using-treezor-as-oauth-identity-provider.html\n- https://docs.treezor.com/guide/cards/_components/tx-authentication-steps.html\n- https://docs.treezor.com/guide/cards/transactions-authentication.html\ndescription: Treezor uses OAuth2 with JWT tokens and Mutual TLS as an additional security layer.\nschemes:\n- type: oauth2\n  name: OAuth2\n  evidence: Treezor leverages the OAuth2 framework and JSON Web Token (JWT) which allows for a wide range of authentication flows.\n  flows:\n  - client_credentials\n  - authorization_code\n  token_url: /oauth/token\n  scopes:\n  - read_only\n  - read_write\n  - admin\n  - keys\n  - legal\n  how_to_obtain: Call the /oauth/token endpoint with client_id and client_secret\
  \ (client_credentials) or exchange an authorization code (authorization_code)\n    to receive a JWT.\n- type: mtls\n  name: Mutual TLS\n  evidence: Treezor also relies on Mutual TLS authentication as an additional security layer.\n  how_to_obtain: Mutual TLS is configured per environment; credentials are provided by Treezor Account Manager.\ndocs: https://docs.treezor.com/guide/api-basics/authentication.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/treezor/refs/heads/main/authentication/treezor-authentication.yml
summary_line: 2 schemes
tags:
- FinTech
- Payments
- Banking-as-a-Service
- API
- Europe
---
