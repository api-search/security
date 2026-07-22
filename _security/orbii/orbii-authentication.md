---
api_key_in: []
api_specs:
- filename: orbii-uae-openapi-original.json
  format: json
  label: Orbii API (UAE)
  slug: orbii-api-uae
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-uae-openapi-original.json
- filename: orbii-ksa-openapi-original.json
  format: json
  label: Orbii KSA API
  slug: orbii-ksa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-ksa-openapi-original.json
- filename: orbii-omn-openapi-original.json
  format: json
  label: Orbii OMN API
  slug: orbii-omn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-omn-openapi-original.json
auth_types:
- query-credentials
description: ''
kind: authentication
layout: security
method: searched
name: Orbii Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orbii secures its APIs with query-credentials across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Orbii
provider_slug: orbii
scheme_count: 1
schemes:
- applies_to: subset of endpoints (e.g. GET /clients)
  documented_in: openapi/orbii-uae-openapi-original.json
  location: query
  name: query-credentials
  parameters:
  - user
  - password
  - client
  type: custom
slug: orbii-authentication
source_filename: orbii-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/orbii-uae-openapi-original.json + api.docs.orbii.ai\nsummary:\n  types: [query-credentials]\n  declared_security_schemes: none\n  note: >-\n    The published OpenAPI specs declare no components.securitySchemes. Auth is\n    handled out-of-band / via credentials passed as query parameters on selected\n    endpoints (user, password) with a 'client' parameter scoping the lender.\nschemes:\n  - name: query-credentials\n    type: custom\n    location: query\n    parameters: [user, password, client]\n    applies_to: subset of endpoints (e.g. GET /clients)\n    documented_in: openapi/orbii-uae-openapi-original.json\nrecommendation: >-\n  Orbii should declare an apiKey or OAuth2 securityScheme and stop accepting\n  credentials in query strings (they leak into logs and browser history).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/authentication/orbii-authentication.yml
summary_line: query-credentials · 1 scheme
tags:
- Company
- Ai
- Lending
- Credit
- Fintech
- Underwriting
- Banking
- SME
- Embedded Finance
- MENA
- Risk
---
