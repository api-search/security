---
anonymous_access: false
api_key_in: []
api_specs:
- filename: brandmov-com-openapi-generated.yml
  format: yaml
  label: BrandMov API
  slug: brandmov-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brandmov-com/openapi/_ae-authored/brandmov-com-openapi-generated.yml
auth_types: []
description: BrandMov API uses a personal API key sent as a bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: BrandMov Authentication
name_suffix: Authentication
oauth_flows: []
overview: BrandMov declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: BrandMov
provider_slug: brandmov-com
scheme_count: 1
schemes:
- evidence: 'Add an Authorization header on every request: curl https://api.brandmov.com/api/v1/watchlists/ \ -H "Authorization: Bearer bm_live_your_key_here"'
  header: Authorization
  how_to_obtain: Mint a key in the dashboard or via POST /account/api-keys; the plaintext key is shown once and used as the bearer token.
  location: header
  name: Bearer
  type: http-bearer
slug: brandmov-com-authentication
source_filename: brandmov-com-authentication.yml
source_heading: Authentication Profile
source_url: https://brandmov.com/docs/api/authentication/
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://brandmov.com/docs/api/authentication/\nsources:\n- https://brandmov.com/docs/api/authentication/\n- https://brandmov.com/docs/api/account/\ndescription: BrandMov API uses a personal API key sent as a bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Add an Authorization header on every request: curl https://api.brandmov.com/api/v1/watchlists/ \\ -H \"Authorization: Bearer bm_live_your_key_here\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Mint a key in the dashboard or via POST /account/api-keys; the plaintext key is shown once and used as the bearer token.\ndocs: https://brandmov.com/docs/api/authentication/\n"
source_yaml_url: https://artifacts.apis.io/brandmov-com/authentication/brandmov-com-authentication.yml
summary_line: 1 scheme
tags:
- Advertising
- Marketing
- Competitive Intelligence
- Software-as-a-Service
- BrandMov
---
