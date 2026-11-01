---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Apifare Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: apifare-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: apifare-com
provider_slug: apifare-com
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Send Authorization: Bearer <token> on every /v1 and /proxy request. Token obtained via POST /v1/signup.'
  scheme: bearer
  type: http
slug: apifare-com-authentication
source_filename: apifare-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://apifare.com/docs\nschemes:\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: \"Send Authorization: Bearer <token> on every /v1 and /proxy request. Token obtained via POST /v1/signup.\"\n"
source_yaml_url: https://artifacts.apis.io/apifare-com/authentication/apifare-com-authentication.yml
summary_line: 1 scheme
tags:
- AI
- Payments
- Prepaid
- Billing
- Agent
---
