---
anonymous_access: false
api_key_in: []
auth_types: []
description: Revolv3 supports static token authentication via the `x-revolv3-token` header and a legacy OAuth2 client‑credentials flow that returns a Bearer token.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Revolv3 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Revolv3 declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Revolv3
provider_slug: revolv3
scheme_count: 1
schemes:
- evidence: Revolv3 authenticates API requests using the `x-revolv3-token` header. The value sent in that header is your **Developer Static Token**.
  header: x-revolv3-token
  how_to_obtain: Create and manage static tokens in the Revolv3 portal under Settings → Integration Profile → Developer Static Tokens.
  location: header
  name: x-revolv3-token
  type: apiKey
slug: revolv3-authentication
source_filename: revolv3-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.revolv3.com/docs/authentication-security/merchant-access-token.md
source_yaml: "generated: '2026-10-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.revolv3.com/docs/authentication-security/merchant-access-token.md\nsources:\n- https://docs.revolv3.com/docs/authentication-security/merchant-access-token.md\n- https://docs.revolv3.com/docs/authentication-security/security-best-practices.md\n- https://docs.revolv3.com/docs/authentication-security/token-faq.md\n- https://docs.revolv3.com/api-reference/authentication/get-merchant-access-token.md\ndescription: Revolv3 supports static token authentication via the `x-revolv3-token` header and a legacy OAuth2 client‑credentials flow that returns\n  a Bearer token.\nschemes:\n- type: apiKey\n  name: x-revolv3-token\n  evidence: Revolv3 authenticates API requests using the `x-revolv3-token` header. The value sent in that header is your **Developer Static Token**.\n  location: header\n  header: x-revolv3-token\n  how_to_obtain: Create and manage static tokens in the Revolv3\
  \ portal under Settings → Integration Profile → Developer Static Tokens.\ndocs: https://docs.revolv3.com/docs/authentication-security/merchant-access-token.md\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/revolv3/authentication/revolv3-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Payments
- SaaS
- Enterprise
- API
---
