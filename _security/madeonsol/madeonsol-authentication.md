---
anonymous_access: false
api_key_in: []
api_specs:
- filename: madeonsol-robinhood-chain-api-openapi.yml
  format: yaml
  label: MadeOnSol Robinhood Chain API
  slug: madeonsol-robinhood-chain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/madeonsol/refs/heads/main/openapi/madeonsol-robinhood-chain-api-openapi.yml
- filename: madeonsol-solana-api-openapi.yml
  format: yaml
  label: MadeOnSol Solana API
  slug: madeonsol-solana-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/madeonsol/refs/heads/main/openapi/madeonsol-solana-api-openapi.yml
auth_types: []
description: MadeOnSol uses a simple API‑key authentication scheme. After signing in, a key is generated on the developer dashboard and must be sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Madeonsol Authentication
name_suffix: Authentication
oauth_flows: []
overview: MadeOnSol declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MadeOnSol
provider_slug: madeonsol
scheme_count: 1
schemes:
- evidence: Your key is generated on the developer dashboard, right after this.
  header: Authorization
  how_to_obtain: Sign in on the MadeOnSol website; a key is generated on the developer dashboard.
  location: header
  name: API Key
  type: http-bearer
slug: madeonsol-authentication
source_filename: madeonsol-authentication.yml
source_heading: Authentication Profile
source_url: https://madeonsol.com/auth/login?next=/developer
source_yaml: "generated: '2026-09-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://madeonsol.com/auth/login?next=/developer\nsources:\n- https://madeonsol.com/auth/login?next=/developer\n- https://madeonsol.com/auth/login?next=%2Fdeveloper\n- https://madeonsol.com/solutions/token-scanners\n- https://madeonsol.com/solutions/token-risk\ndescription: MadeOnSol uses a simple API‑key authentication scheme. After signing in, a key is generated on the developer dashboard and must be\n  sent as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: Your key is generated on the developer dashboard, right after this.\n  location: header\n  header: Authorization\n  how_to_obtain: Sign in on the MadeOnSol website; a key is generated on the developer dashboard.\nnote: No OAuth2, apiKey, or other authentication methods are documented on the provided pages.\ndocs: https://madeonsol.com/auth/login?next=/developer\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/madeonsol/refs/heads/main/authentication/madeonsol-authentication.yml
summary_line: 1 scheme
tags:
- Blockchain
- Analytics
- Solana
- Robinhood Chain
- API
---
