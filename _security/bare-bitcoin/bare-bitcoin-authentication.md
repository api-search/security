---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bare-bitcoin-developers-openapi.json
  format: json
  label: Bare Bitcoin API Developers API
  slug: bare-bitcoin-api-developers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bare-bitcoin/openapi/_original/bare-bitcoin-developers-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Bare Bitcoin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bare Bitcoin declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Bare Bitcoin
provider_slug: bare-bitcoin
scheme_count: 2
schemes:
- evidence: Send the complete key in x-bb-api-key.
  header: x-bb-api-key
  how_to_obtain: Create a key in API‑key settings (the key starts with bb/public/ and the secret starts with bb/apisecret/).
  location: header
  name: API key
  type: apiKey
- authorize_url: https://barebitcoin.no/oauth2/authorize
  evidence: 'Send the token as Authorization: Bearer <access token>.'
  flows:
  - authorization_code
  - refresh_token
  header: Authorization
  how_to_obtain: Contact Bare Bitcoin to arrange client registration and obtain a client_id (and client_secret for confidential clients).
  location: header
  name: OAuth
  scopes:
  - api:accounts:bitcoin:read
  - api:trades:read
  - api:tax:transactions:read
  - api:deposits:lightning:read
  - api:deposits:lightning:write
  type: oauth2
slug: bare-bitcoin-authentication
source_filename: bare-bitcoin-authentication.yml
source_heading: Authentication Profile
source_url: https://barebitcoin.no/developers/authentication
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://barebitcoin.no/developers/authentication\nsources:\n- https://barebitcoin.no/developers/authentication\n- https://barebitcoin.no/developers/authentication/api-keys\n- https://barebitcoin.no/developers/authentication/oauth\n- https://barebitcoin.no/developers/authentication.md\nschemes:\n- type: apiKey\n  name: API key\n  evidence: Send the complete key in x-bb-api-key.\n  location: header\n  header: x-bb-api-key\n  how_to_obtain: Create a key in API‑key settings (the key starts with bb/public/ and the secret starts with bb/apisecret/).\n- type: oauth2\n  name: OAuth\n  evidence: 'Send the token as Authorization: Bearer <access token>.'\n  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  - refresh_token\n  authorize_url: https://barebitcoin.no/oauth2/authorize\n  scopes:\n  - api:accounts:bitcoin:read\n  - api:trades:read\n  - api:tax:transactions:read\n\
  \  - api:deposits:lightning:read\n  - api:deposits:lightning:write\n  how_to_obtain: Contact Bare Bitcoin to arrange client registration and obtain a client_id (and client_secret for confidential clients).\ndocs: https://barebitcoin.no/developers/authentication\n"
source_yaml_url: https://artifacts.apis.io/bare-bitcoin/authentication/bare-bitcoin-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Cryptocurrency
- Finance
- Payments
- Norway
---
