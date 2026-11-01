---
anonymous_access: false
api_key_in: []
api_specs:
- filename: farmready-openapi-generated.yml
  format: yaml
  label: FarmReady (Bolt, Cart, Shed) API
  slug: farmready-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/farmready/openapi/_ae-authored/farmready-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Farmready Authentication
name_suffix: Authentication
oauth_flows: []
overview: FarmReady (Bolt, Cart, Shed) declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: FarmReady (Bolt, Cart, Shed)
provider_slug: farmready
scheme_count: 1
schemes:
- description: Bearer token authentication; token prefixed with "fr_" and issued per customer account.
  in: header
  name: Authorization
  prefix: fr_
  type: bearer
slug: farmready-authentication
source_filename: farmready-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: searched\nsource: https://www.farmready.io/developer/docs/authentication\nschemes:\n  - type: bearer\n    name: Authorization\n    in: header\n    prefix: fr_\n    description: Bearer token authentication; token prefixed with \"fr_\" and issued per customer account.\n"
source_yaml_url: https://artifacts.apis.io/farmready/authentication/farmready-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Agriculture
- Farm Management
- Inventory
- Equipment
- Safety
---
