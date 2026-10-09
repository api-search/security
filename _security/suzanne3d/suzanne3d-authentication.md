---
anonymous_access: false
api_key_in: []
api_specs:
- filename: suzanne3d-openapi-generated.yml
  format: yaml
  label: Suzanne API
  slug: suzanne-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suzanne3d/refs/heads/main/openapi/_ae-authored/suzanne3d-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Suzanne3D Authentication
name_suffix: Authentication
oauth_flows: []
overview: Suzanne declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Suzanne
provider_slug: suzanne3d
scheme_count: 1
schemes:
- applies_to: all operations
  docs: https://console.suzanne3d.com/documentation/authentication
  format: Bearer sznn_test_xxx | Bearer sznn_live_xxx
  header: Authorization
  in: header
  issued_from: https://console.suzanne3d.com/dashboard
  key_prefixes:
    production: sznn_live_
    sandbox: sznn_test_
  name: bearer
  scheme: bearer
  statement: 'Every request requires a Bearer token issued to your account. Keys start with sznn_test_ (sandbox) or sznn_live_ (production). Treat them like a password: server-side only, never in client code.'
  type: http
slug: suzanne3d-authentication
source_filename: suzanne3d-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: searched\nsource: https://console.suzanne3d.com/documentation/authentication\ndocs: https://console.suzanne3d.com/documentation/authentication\nsummary: Every Suzanne API request is authenticated with a Bearer API key issued to the account; keys are prefixed\n  sznn_test_ (sandbox) or sznn_live_ (production) and are server-side only. No OAuth, no scopes reference page (a\n  403 forbidden_scope error is documented, so keys do carry scopes, but none are enumerated).\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: Bearer sznn_test_xxx | Bearer sznn_live_xxx\n  key_prefixes:\n    sandbox: sznn_test_\n    production: sznn_live_\n  statement: 'Every request requires a Bearer token issued to your account. Keys start with sznn_test_ (sandbox)\n    or sznn_live_ (production). Treat them like a password: server-side only, never in client code.'\n  issued_from: https://console.suzanne3d.com/dashboard\n\
  \  applies_to: all operations\n  docs: https://console.suzanne3d.com/documentation/authentication\nerrors:\n- status: 401\n  code: unauthorized\n  meaning: Missing / bad API key.\n- status: 403\n  code: forbidden_scope\n  meaning: Key lacks the required scope.\noauth: false\nscopes_documented: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/suzanne3d/refs/heads/main/authentication/suzanne3d-authentication.yml
summary_line: 1 scheme
tags:
- Company
- 3D
- 3D Models
- Generative AI
- Industrial Design
- CAD
- Mesh Generation
- Text-to-3D
- Photo-to-3D
- Manufacturing
---
