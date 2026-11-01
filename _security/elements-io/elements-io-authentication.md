---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Circle APIs and user‑controlled wallets
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Elements Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Elements declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Elements
provider_slug: elements-io
scheme_count: 1
schemes:
- evidence: API key required. Bearer token in Authorization header.
  header: Authorization
  how_to_obtain: Create an API key in the Circle Console and use its value as a Bearer token.
  location: header
  name: API Key
  type: http-bearer
slug: elements-io-authentication
source_filename: elements-io-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.circle.com/wallets/user-controlled/authentication-methods.md
source_yaml: "generated: '2026-10-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.circle.com/wallets/user-controlled/authentication-methods.md\nsources:\n- https://developers.circle.com/wallets/user-controlled/authentication-methods.md\n- https://developers.circle.com/contracts/create-api-key.md\n- https://developers.circle.com/wallets/signing-and-authorization-models.md\n- https://developers.circle.com/wallets/dev-controlled/transfer-tokens-across-wallets.md\ndescription: Authentication methods for Circle APIs and user‑controlled wallets\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: API key required. Bearer token in Authorization header.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the Circle Console and use its value as a Bearer token.\ndocs: https://developers.circle.com/wallets/user-controlled/authentication-methods.md\n"
source_yaml_url: https://artifacts.apis.io/elements-io/authentication/elements-io-authentication.yml
summary_line: 1 scheme
tags:
- Stablecoins
- Digital Assets
- Payments
- Treasury Management
- Developer Services
- Trading Services
---
