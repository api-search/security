---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bloq-openapi-generated.yml
  format: yaml
  label: Bloq API
  slug: bloq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloq/refs/heads/main/openapi/_ae-authored/bloq-openapi-generated.yml
auth_types: []
description: Authentication methods for Bloq services
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Bloq Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bloq declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Bloq
provider_slug: bloq
scheme_count: 2
schemes:
- evidence: To authorize the requests, a bearer JSON Web Token must be sent in the Authorization header.
  header: Authorization
  how_to_obtain: Obtain a JWT token via the Bloq authentication flow (e.g., nonce‑signature flow or client token endpoint) and include it as `Bearer <token>` in the Authorization header.
  location: header
  name: Bearer JWT
  type: http-bearer
- evidence: Using HTTP Basic Authentication by providing username (User ID or email) and password, this endpoint retrieves an authentication token to be passed to other Accounts API functions for authentication.
  header: Authorization
  how_to_obtain: Send a POST request to https://api.bloq.com/auth/login with `-u username:password` to receive an authentication token.
  location: header
  name: Basic Authentication
  token_url: https://api.bloq.com/auth/login
  type: http-basic
slug: bloq-authentication
source_filename: bloq-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.bloq.com/bloq-services/bloqstake/authenticate-to-bloq-api/authentication.md
source_yaml: "generated: '2026-09-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.bloq.com/bloq-services/bloqstake/authenticate-to-bloq-api/authentication.md\nsources:\n- https://docs.bloq.com/bloq-services/bloqstake/authenticate-to-bloq-api/authentication.md\n- https://docs.bloq.com/advanced-documentation/developers-guide/authentication.md\n- https://docs.bloq.com/advanced-documentation/developers-guide/client-tokens.md\n- https://docs.bloq.com/readme/bloq-account-setup.md\ndescription: Authentication methods for Bloq services\nschemes:\n- type: http-bearer\n  name: Bearer JWT\n  evidence: To authorize the requests, a bearer JSON Web Token must be sent in the Authorization header.\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain a JWT token via the Bloq authentication flow (e.g., nonce‑signature flow or client token endpoint) and include it as `Bearer\n    <token>` in the Authorization header.\n- type: http-basic\n  name: Basic\
  \ Authentication\n  evidence: Using HTTP Basic Authentication by providing username (User ID or email) and password, this endpoint retrieves an authentication token\n    to be passed to other Accounts API functions for authentication.\n  location: header\n  header: Authorization\n  token_url: https://api.bloq.com/auth/login\n  how_to_obtain: Send a POST request to https://api.bloq.com/auth/login with `-u username:password` to receive an authentication token.\ndocs: https://docs.bloq.com/bloq-services/bloqstake/authenticate-to-bloq-api/authentication.md\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloq/refs/heads/main/authentication/bloq-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Web3
- Infrastructure
- DeFi
- Blockchain
---
