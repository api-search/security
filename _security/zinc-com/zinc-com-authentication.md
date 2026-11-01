---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Zinc Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zinc declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Zinc
provider_slug: zinc-com
scheme_count: 1
schemes:
- evidence: Authentication is performed using Bearer token authentication . Include your API key in the Authorization header
  header: Authorization
  how_to_obtain: Find your API key in your Zinc dashboard after creating an account.
  location: header
  name: Bearer
  type: http-bearer
slug: zinc-com-authentication
source_filename: zinc-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.zinc.com/docs/v2/api-reference/introduction/authentication
source_yaml: "generated: '2026-10-24'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.zinc.com/docs/v2/api-reference/introduction/authentication\nsources:\n- https://www.zinc.com/docs/v2/api-reference/introduction/authentication\n- https://www.zinc.com/docs/v2/api-reference/device/redeem-device-code\n- https://www.zinc.com/docs/quickstart\n- https://www.zinc.com/blog/mpp\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Authentication is performed using Bearer token authentication . Include your API key in the Authorization header\n  location: header\n  header: Authorization\n  how_to_obtain: Find your API key in your Zinc dashboard after creating an account.\ndocs: https://www.zinc.com/docs/v2/api-reference/introduction/authentication\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/zinc-com/authentication/zinc-com-authentication.yml
summary_line: 1 scheme
tags:
- E‑commerce API
- Product Search
- Order Automation
- Retail Integration
- Procurement
---
