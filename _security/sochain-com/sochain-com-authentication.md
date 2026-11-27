---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication is performed by sending an API key.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: sochain-com Authentication
name_suffix: Authentication
oauth_flows: []
overview: sochain-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: sochain-com
provider_slug: sochain-com
scheme_count: 1
schemes:
- evidence: Send your API key in the API-KEY header (lookups also work without one).
  header: API-KEY
  how_to_obtain: Sign in with your email, receive an 8‑digit code, and copy the key shown on the dashboard.
  location: header
  name: API-KEY
  type: apiKey
slug: sochain-com-authentication
source_filename: sochain-com-authentication.yml
source_heading: Authentication Profile
source_url: https://sochain.com/docs/authentication
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://sochain.com/docs/authentication\nsources:\n- https://sochain.com/docs/authentication\n- https://dev.sochain.com/signin\n- https://dev.sochain.com/signin?next=%2Fdashboard\n- https://sochain.com/docs\ndescription: Authentication is performed by sending an API key.\nschemes:\n- type: apiKey\n  name: API-KEY\n  evidence: Send your API key in the API-KEY header (lookups also work without one).\n  location: header\n  header: API-KEY\n  how_to_obtain: Sign in with your email, receive an 8‑digit code, and copy the key shown on the dashboard.\nnote: 'The header can also be sent as X-API-Key or Authorization: Bearer, but the primary documented name is API-KEY.'\ndocs: https://sochain.com/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/sochain-com/authentication/sochain-com-authentication.yml
summary_line: 1 scheme
tags:
- Blockchain
- Explorer
- Bitcoin
- Litecoin
- Dogecoin
- Zcash
---
