---
anonymous_access: false
api_key_in: []
api_specs:
- filename: billdog-io-openapi-generated.yml
  format: yaml
  label: BillDog API
  slug: billdog-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/billdog-io/openapi/_ae-authored/billdog-io-openapi-generated.yml
auth_types: []
description: BillDog Auth endpoints are authenticated using a public API key.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: BillDog Authentication
name_suffix: Authentication
oauth_flows: []
overview: BillDog declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: BillDog
provider_slug: billdog-io
scheme_count: 1
schemes:
- evidence: 'The key is read from `X-BillDog-API-Key` only — never from `Authorization: Bearer` or the query string.'
  header: X-BillDog-API-Key
  how_to_obtain: Obtain a public key (`bd_public_*`) from the BillDog dashboard; it is shipped in the client app.
  location: header
  name: Public API Key
  type: apiKey
slug: billdog-io-authentication
source_filename: billdog-io-authentication.yml
source_heading: Authentication Profile
source_url: https://billdog.io/docs/auth/mfa.md
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://billdog.io/docs/auth/mfa.md\nsources:\n- https://billdog.io/docs/auth/mfa.md\n- https://billdog.io/docs/stripe-integration\n- https://billdog.io/docs/auth.md\n- https://billdog.io/docs/auth/api-reference.md\ndescription: BillDog Auth endpoints are authenticated using a public API key.\nschemes:\n- type: apiKey\n  name: Public API Key\n  evidence: 'The key is read from `X-BillDog-API-Key` only — never from `Authorization: Bearer` or the query string.'\n  location: header\n  header: X-BillDog-API-Key\n  how_to_obtain: Obtain a public key (`bd_public_*`) from the BillDog dashboard; it is shipped in the client app.\nnote: No OAuth2, HTTP Bearer, HTTP Basic, JWT, HMAC, mTLS, or other schemes are documented on the provided pages.\ndocs: https://billdog.io/docs/auth/mfa.md\n"
source_yaml_url: https://artifacts.apis.io/billdog-io/authentication/billdog-io-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Analytics
- Monetization
- Software-as-a-Service
- Platform
- Company
---
