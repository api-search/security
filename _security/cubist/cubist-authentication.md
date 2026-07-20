---
api_key_in:
- header
api_specs:
- filename: cubist-cubesigner-openapi-original.json
  format: json
  label: CubeSigner API
  slug: cubist-cubesigner
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cubist/refs/heads/main/openapi/cubist-cubesigner-openapi-original.json
auth_types:
- oidc-exchange
- session-token
description: ''
kind: authentication
layout: security
method: searched
name: Cubist Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cubist secures its APIs with oidc-exchange and session-token across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cubist
provider_slug: cubist
scheme_count: 2
schemes:
- description: OIDC tokens authenticate users via a third-party identity provider and are exchanged for signer session tokens.
  in: header
  name: Oidc
  parameter: Authorization
  sources:
  - openapi/cubist-cubesigner-openapi-original.json
  type: bearer
- description: Signer session tokens authenticate signing endpoints. Created with `cs token create` (or the SDK); scoped and time-bounded.
  in: header
  name: SignerAuth
  parameter: Authorization
  sources:
  - openapi/cubist-cubesigner-openapi-original.json
  type: bearer
slug: cubist-authentication
source_filename: cubist-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/cubist-cubesigner-openapi-original.json\ndocs: https://cubist.dev/product-suite\nsummary:\n  types: [oidc-exchange, session-token]\n  api_key_in: [header]\n  model: >-\n    Two-stage: an OIDC identity token authenticates the user and is exchanged for\n    a CubeSigner signer session token; signing endpoints then require that\n    session token. Both are carried in the Authorization header. Sessions and\n    Role access tokens carry a bounded scope set (see scopes/).\n  mfa: [email-otp, totp, fido/passkey]\nschemes:\n  - name: Oidc\n    type: bearer\n    in: header\n    parameter: Authorization\n    description: >-\n      OIDC tokens authenticate users via a third-party identity provider and are\n      exchanged for signer session tokens.\n    sources: [openapi/cubist-cubesigner-openapi-original.json]\n  - name: SignerAuth\n    type: bearer\n    in: header\n    parameter: Authorization\n    description: >-\n      Signer\
  \ session tokens authenticate signing endpoints. Created with\n      `cs token create` (or the SDK); scoped and time-bounded.\n    sources: [openapi/cubist-cubesigner-openapi-original.json]\nscopes_reference: scopes/cubist-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cubist/refs/heads/main/authentication/cubist-authentication.yml
summary_line: oidc-exchange/session-token · 2 schemes
tags:
- Company
- Developer Tools
- Key Management
- Wallets
- Digital Signatures
- Security
- Blockchain
- Web3
- Custody
---
