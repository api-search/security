---
anonymous_access: false
api_key_in: []
api_specs:
- filename: inttegro-com-openapi-generated.yml
  format: yaml
  label: Inttegro API
  slug: inttegro-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inttegro-com/openapi/_ae-authored/inttegro-com-openapi-generated.yml
auth_types: []
description: Inttegro authenticates API requests with an opaque bearer key. Keep the key in server-side secret storage and include it in the Authorization header for every request.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Inttegro Authentication
name_suffix: Authentication
oauth_flows: []
overview: Inttegro declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Inttegro
provider_slug: inttegro-com
scheme_count: 1
schemes:
- evidence: Inttegro authenticates API requests with an opaque bearer key. Keep the key in server-side secret storage and include it in the Authorization header for every request.
  header: Authorization
  how_to_obtain: Generate a secret key via POST /keys/generate; the token is returned once in the response.
  location: header
  name: Bearer
  type: http-bearer
slug: inttegro-com-authentication
source_filename: inttegro-com-authentication.yml
source_heading: Authentication Profile
source_url: https://studio.inttegro.dev/api/authentication
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://studio.inttegro.dev/api/authentication\nsources:\n- https://studio.inttegro.dev/api/authentication\n- https://studio.inttegro.dev/api/keys\n- https://studio.inttegro.dev/e/c-authentication_failed\n- https://studio.inttegro.dev/api/authentication\ndescription: Inttegro authenticates API requests with an opaque bearer key. Keep the key in server-side secret storage and include it in the Authorization\n  header for every request.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Inttegro authenticates API requests with an opaque bearer key. Keep the key in server-side secret storage and include it in the Authorization\n    header for every request.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate a secret key via POST /keys/generate; the token is returned once in the response.\ndocs: https://studio.inttegro.dev/api/authentication\n"
source_yaml_url: https://artifacts.apis.io/inttegro-com/authentication/inttegro-com-authentication.yml
summary_line: 1 scheme
tags:
- Commerce
- Payments
- Software-as-a-Service
- E-Commerce
---
