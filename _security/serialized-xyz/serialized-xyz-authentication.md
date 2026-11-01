---
anonymous_access: false
api_key_in: []
auth_types: []
description: Serialized API uses a simple API key.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Serialized Xyz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Serialized declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Serialized
provider_slug: serialized-xyz
scheme_count: 1
schemes:
- evidence: 'Pass your raw API key in the `Authorization` header on every request (same convention as Mobula, zero migration friction). No `Bearer` prefix: the header value is the key itself.'
  header: Authorization
  how_to_obtain: Create an account, add a payment method, then create API keys in the portal.
  location: header
  name: apiKey
  type: apiKey
slug: serialized-xyz-authentication
source_filename: serialized-xyz-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.serialized.xyz/authentication.md
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.serialized.xyz/authentication.md\nsources:\n- https://docs.serialized.xyz/authentication.md\n- https://docs.serialized.xyz/endpoints/token-search.md\n- https://docs.serialized.xyz/endpoints/token-details.md\n- https://docs.serialized.xyz/endpoints/token-details-batch.md\ndescription: Serialized API uses a simple API key.\nschemes:\n- type: apiKey\n  name: apiKey\n  evidence: 'Pass your raw API key in the `Authorization` header on every request (same convention as Mobula, zero migration friction). No `Bearer`\n    prefix: the header value is the key itself.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an account, add a payment method, then create API keys in the portal.\ndocs: https://docs.serialized.xyz/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/serialized-xyz/authentication/serialized-xyz-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Onchain
- MarketData
- TokenSecurity
- API
- Data
---
