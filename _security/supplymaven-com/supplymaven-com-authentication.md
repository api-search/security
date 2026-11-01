---
anonymous_access: false
api_key_in: []
api_specs:
- filename: supplymaven-com-openapi-generated.yml
  format: yaml
  label: supplymaven-com API
  slug: supplymaven-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/supplymaven-com/openapi/_ae-authored/supplymaven-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Supplymaven Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: supplymaven-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: supplymaven-com
provider_slug: supplymaven-com
scheme_count: 1
schemes:
- description: Bearer token in Authorization header. Keys prefixed by tier (sm_free_, sm_live_). Free keys for free tier, paid keys for Pro/Signal.
  header: Authorization
  token_prefixes:
  - sm_free_
  - sm_live_
  type: bearer
slug: supplymaven-com-authentication
source_filename: supplymaven-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://supplymaven.com/developers/docs\nschemes:\n  - type: bearer\n    description: Bearer token in Authorization header. Keys prefixed by tier (sm_free_, sm_live_). Free keys for free tier, paid keys for Pro/Signal.\n    header: Authorization\n    token_prefixes:\n      - sm_free_\n      - sm_live_"
source_yaml_url: https://artifacts.apis.io/supplymaven-com/authentication/supplymaven-com-authentication.yml
summary_line: 1 scheme
tags:
- Supply Chain
- Risk Intelligence
- Data Platform
- Analytics
- Logistics
---
