---
anonymous_access: false
api_key_in: []
api_specs:
- filename: flyn-to-openapi-generated.yml
  format: yaml
  label: Flyn API
  slug: flyn-to-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyn-to/openapi/_ae-authored/flyn-to-openapi-generated.yml
auth_types: []
description: Authentication schemes published on Flyn documentation.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Flyn To Authentication
name_suffix: Authentication
oauth_flows: []
overview: Flyn declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Flyn
provider_slug: flyn-to
scheme_count: 1
schemes:
- evidence: The Flyn API uses Bearer-token authentication. Every request must include a valid API key in the Authorization header.
  header: Authorization
  how_to_obtain: Generate an API key in the Flyn dashboard (Settings → API) and use it as the Bearer token.
  location: header
  name: Bearer token
  type: http-bearer
slug: flyn-to-authentication
source_filename: flyn-to-authentication.yml
source_heading: Authentication Profile
source_url: https://www.flyn.to/docs/authentication
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.flyn.to/docs/authentication\nsources:\n- https://www.flyn.to/docs/authentication\n- https://www.flyn.to/docs/shorten\n- https://www.flyn.to/blog/qr-codes-for-restaurant-menus\ndescription: Authentication schemes published on Flyn documentation.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: The Flyn API uses Bearer-token authentication. Every request must include a valid API key in the Authorization header.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API key in the Flyn dashboard (Settings → API) and use it as the Bearer token.\ndocs: https://www.flyn.to/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/flyn-to/authentication/flyn-to-authentication.yml
summary_line: 1 scheme
tags:
- link shortener
- URL analytics
- branded domains
- API
- QR codes
- team workspaces
- A/B testing
- developer tools
---
