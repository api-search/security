---
anonymous_access: false
api_key_in: []
api_specs:
- filename: polly-io-openapi-generated.yml
  format: yaml
  label: Polly API
  slug: polly-io-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polly-io/refs/heads/main/openapi/_ae-authored/polly-io-openapi-generated.yml
auth_types: []
description: Polly uses an OAuth 2.0‑style Resource Owner Password Credentials (ROPC) flow to issue short‑lived access tokens.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Polly Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Polly declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Polly
provider_slug: polly-io
scheme_count: 2
schemes:
- evidence: Polly uses an OAuth 2.0–style Resource Owner Password Credentials (ROPC) flow to issue short-lived access tokens.
  flows:
  - password
  how_to_obtain: POST https://api.prod.polly.io/api/v2/auth/token/ with form‑encoded body parameters username, password, client_id, client_secret and grant_type=password.
  name: Polly OAuth2
  scopes:
  - write
  - read
  token_url: https://api.prod.polly.io/api/v2/auth/token/
  type: oauth2
- evidence: 'Include your bearer token in the header of every API request: Authorization: Bearer YOUR_ACCESS_TOKEN'
  header: Authorization
  how_to_obtain: Obtain the token via the OAuth2 password flow described above and then send it in the Authorization header as "Bearer <token>".
  location: header
  name: Bearer token
  type: http-bearer
slug: polly-io-authentication
source_filename: polly-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.polly.io/docs/authentication.md
source_yaml: "generated: '2026-10-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.polly.io/docs/authentication.md\nsources:\n- https://docs.polly.io/docs/authentication.md\n- https://docs.polly.io/reference/securityoauthretrieve.md\n- https://docs.polly.io/reference/securityoauthcreate.md\n- https://docs.polly.io/reference/securityoauthpartialupdate.md\ndescription: Polly uses an OAuth 2.0‑style Resource Owner Password Credentials (ROPC) flow to issue short‑lived access tokens.\nschemes:\n- type: oauth2\n  name: Polly OAuth2\n  evidence: Polly uses an OAuth 2.0–style Resource Owner Password Credentials (ROPC) flow to issue short-lived access tokens.\n  flows:\n  - password\n  token_url: https://api.prod.polly.io/api/v2/auth/token/\n  scopes:\n  - write\n  - read\n  how_to_obtain: POST https://api.prod.polly.io/api/v2/auth/token/ with form‑encoded body parameters username, password, client_id, client_secret\n    and grant_type=password.\n- type: http-bearer\n\
  \  name: Bearer token\n  evidence: 'Include your bearer token in the header of every API request: Authorization: Bearer YOUR_ACCESS_TOKEN'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain the token via the OAuth2 password flow described above and then send it in the Authorization header as \"Bearer <token>\".\ndocs: https://docs.polly.io/docs/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polly-io/refs/heads/main/authentication/polly-io-authentication.yml
summary_line: 2 schemes
tags:
- FinTech
- CapitalMarkets
- Mortgage
- APIPlatform
- AI
---
