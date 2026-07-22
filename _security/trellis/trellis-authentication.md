---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Trellis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trellis secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Trellis
provider_slug: trellis
scheme_count: 1
schemes:
- description: API-key credentials issued to Trellis API customers. Details provided during onboarding.
  in: header
  name: ApiKey
  sources:
  - https://support.trellis.law/trellis-api
  type: apiKey
slug: trellis-authentication
source_filename: trellis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://support.trellis.law/trellis-api\ndocs: https://support.trellis.law/trellis-api\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Trellis authenticates API requests with issued API credentials (key-based),\n    provisioned when a customer begins a free trial via Trellis Sales. The full\n    authentication reference (exact header names, key rotation, temporary\n    client-side access keys vs. backend secret keys) is gated behind API\n    onboarding and is not published on the public developer surface.\nschemes:\n  - name: ApiKey\n    type: apiKey\n    in: header\n    description: >-\n      API-key credentials issued to Trellis API customers. Details provided\n      during onboarding.\n    sources: [https://support.trellis.law/trellis-api]\naccess:\n  model: sales-gated free trial\n  contact: sales@trellis.law\nnotes: >-\n  No OpenAPI/Swagger spec is published publicly, so this\
  \ profile is searched\n  from docs rather than derived from a spec. There is no OAuth2 scope surface\n  documented; scopes/ is intentionally omitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trellis/refs/heads/main/authentication/trellis-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Legal
- Legal Analytics
- Court Data
- Litigation
- Legal Tech
- Judicial Analytics
- Artificial Intelligence
---
