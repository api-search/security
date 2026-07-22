---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Virgil Security Authentication
name_suffix: Authentication
oauth_flows: []
overview: Virgil Security secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Virgil Security
provider_slug: virgil-security
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Short-lived JWT signed by the application''s Virgil API Key and presented as `Authorization: Bearer <jwt>` to Virgil Cloud services.'
  name: virgilJwt
  scheme: bearer
  sources:
  - docs
  type: http
slug: virgil-security-authentication
source_filename: virgil-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.virgilsecurity.com/docs/e3kit/fundamentals/jwt/\ndocs: https://developer.virgilsecurity.com/docs/platform/api-reference/\nnotes: >-\n  No OpenAPI is published for the Virgil service APIs (Cards, Keyknox, Pythia,\n  PFS), so this profile is derived from the developer documentation rather than\n  a spec. Virgil services authenticate with a short-lived JSON Web Token (JWT).\n  The JWT is generated server-side by the application backend using the app's\n  Virgil App ID, API Key ID and API Key (private key) obtained from the Virgil\n  Dashboard; the client SDK requests this JWT from the backend and presents it\n  to Virgil Cloud services as a Bearer token. Account/application and API-key\n  management is done via the Virgil Dashboard and the virgil-cli tool.\nsummary:\n  types: [http]\n  scheme: bearer\n  bearer_format: JWT\n  token_issuance: server-side (application backend)\n  credentials_source: Virgil Dashboard\
  \ (App ID + API Key ID + API Key)\nschemes:\n  - name: virgilJwt\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      Short-lived JWT signed by the application's Virgil API Key and presented\n      as `Authorization: Bearer <jwt>` to Virgil Cloud services.\n    sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virgil-security/refs/heads/main/authentication/virgil-security-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Encryption
- End-to-End Encryption
- Cryptography
- Key Management
- Authentication
- Passwords
- IoT Security
- Developer Tools
---
