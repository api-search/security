---
anonymous_access: false
api_key_in: []
api_specs:
- filename: l1nk-website-openapi-generated.yml
  format: yaml
  label: L1NK API
  slug: l1nk-website-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/l1nk-website/openapi/_ae-authored/l1nk-website-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: L1NK Authentication
name_suffix: Authentication
oauth_flows: []
overview: L1NK declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: L1NK
provider_slug: l1nk-website
scheme_count: 1
schemes:
- evidence: 'Send it in the Authorization: Bearer … header, as in the example.'
  header: Authorization
  how_to_obtain: Generate token in the dashboard (Account → API) and copy it.
  location: header
  name: Bearer token
  type: http-bearer
slug: l1nk-website-authentication
source_filename: l1nk-website-authentication.yml
source_heading: Authentication Profile
source_url: https://l1nk.website/en/solutions/developers
source_yaml: "generated: '2026-11-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://l1nk.website/en/solutions/developers\nsources:\n- https://l1nk.website/en/solutions/developers\n- https://l1nk.website/en/help/api\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Send it in the Authorization: Bearer … header, as in the example.'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate token in the dashboard (Account → API) and copy it.\ndocs: https://l1nk.website/en/solutions/developers\n"
source_yaml_url: https://artifacts.apis.io/l1nk-website/authentication/l1nk-website-authentication.yml
summary_line: 1 scheme
tags:
- Short Links
- URL Shorteners
- Analytics
- QR Codes
- AI Integration
---
