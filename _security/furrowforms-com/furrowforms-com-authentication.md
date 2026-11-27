---
anonymous_access: false
api_key_in: []
api_specs:
- filename: furrowforms-com-openapi-generated.yml
  format: yaml
  label: Furrow Forms API
  slug: furrowforms-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/furrowforms-com/openapi/_ae-authored/furrowforms-com-openapi-generated.yml
auth_types: []
description: Furrow Forms uses a bearer token (the `frw_` token) that is minted after registering an account and verifying a 6‑digit email code.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Furrow Forms Authentication
name_suffix: Authentication
oauth_flows: []
overview: Furrow Forms declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Furrow Forms
provider_slug: furrowforms-com
scheme_count: 1
schemes:
- evidence: it registers your account over GET/POST /api/register, verifies your email, and mints its own token.
  header: Authorization
  how_to_obtain: Register via POST https://api.furrowforms.com/api/register, read the 6‑digit verification code from the email, and mint a token.
  location: header
  name: Bearer
  type: http-bearer
slug: furrowforms-com-authentication
source_filename: furrowforms-com-authentication.yml
source_heading: Authentication Profile
source_url: https://furrowforms.com/ai
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://furrowforms.com/ai\nsources:\n- https://furrowforms.com/ai\ndescription: Furrow Forms uses a bearer token (the `frw_` token) that is minted after registering an account and verifying a 6‑digit email code.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: it registers your account over GET/POST /api/register, verifies your email, and mints its own token.\n  location: header\n  header: Authorization\n  how_to_obtain: Register via POST https://api.furrowforms.com/api/register, read the 6‑digit verification code from the email, and mint a token.\nnote: No OAuth2 flows, API‑key, or other authentication schemes are documented on the page.\ndocs: https://furrowforms.com/ai\n"
source_yaml_url: https://artifacts.apis.io/furrowforms-com/authentication/furrowforms-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Forms
- Backend
- Artificial Intelligence
- Integration
---
