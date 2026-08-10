---
api_key_in:
- header
api_specs:
- filename: aquabyte-behaviour-api-openapi.yml
  format: yaml
  label: Aquabyte Behaviour API
  slug: aquabyte-behaviour-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquabyte/refs/heads/main/openapi/aquabyte-behaviour-api-openapi.yml
- filename: aquabyte-biomass-api-openapi.yml
  format: yaml
  label: Aquabyte Biomass API
  slug: aquabyte-biomass-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquabyte/refs/heads/main/openapi/aquabyte-biomass-api-openapi.yml
- filename: aquabyte-environmental-api-openapi.yml
  format: yaml
  label: Aquabyte Environmental API
  slug: aquabyte-environmental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquabyte/refs/heads/main/openapi/aquabyte-environmental-api-openapi.yml
- filename: aquabyte-lice-api-openapi.yml
  format: yaml
  label: Aquabyte Lice API
  slug: aquabyte-lice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquabyte/refs/heads/main/openapi/aquabyte-lice-api-openapi.yml
- filename: aquabyte-sites-api-openapi.yml
  format: yaml
  label: Aquabyte Sites API
  slug: aquabyte-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquabyte/refs/heads/main/openapi/aquabyte-sites-api-openapi.yml
- filename: aquabyte-v3-0-api-openapi.yml
  format: yaml
  label: Aquabyte V3.0 API
  slug: aquabyte-v3-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquabyte/refs/heads/main/openapi/aquabyte-v3-0-api-openapi.yml
- filename: aquabyte-welfare-api-openapi.yml
  format: yaml
  label: Aquabyte Welfare API
  slug: aquabyte-welfare-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquabyte/refs/heads/main/openapi/aquabyte-welfare-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Aquabyte Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aquabyte secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Aquabyte
provider_slug: aquabyte
scheme_count: 1
schemes:
- applies_to: all operations
  description: 'Per-customer API key issued by Aquabyte. Sent on every HTTPS request as the `apikey` request header. Quoted verbatim from the published API description: "To use our API you must be issued an API key. Instructions: For all HTTPS requests you will need to pass in your API key as part of the header: `apikey: {API_KEY}`".'
  in: header
  issuance: manual — keys are issued by Aquabyte to existing customers; there is no public self-service signup for API credentials.
  name: apikey
  parameter_name: apikey
  sources:
  - https://api.aquabyte.ai/openapi.json (info.description)
  type: apiKey
slug: aquabyte-authentication
source_filename: aquabyte-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: https://api.aquabyte.ai/openapi.json\ndocs: https://api.aquabyte.ai/v3/docs\nnote: >-\n  The OpenAPI 3.1 document Aquabyte serves at api.aquabyte.ai/openapi.json declares NO\n  components.securitySchemes and no top-level security requirement — the auth contract is\n  documented in prose inside info.description instead. This profile is therefore SEARCHED\n  from that published description (and confirmed by probing a protected operation), not\n  derived from securitySchemes. The gap is worth reporting to the provider: adding an\n  apiKey securityScheme and applying it would make the contract machine-readable.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  spec_declares_security_schemes: false\nschemes:\n- name: apikey\n  type: apiKey\n  in: header\n  parameter_name: apikey\n  description: >-\n    Per-customer API key issued by Aquabyte. Sent on every HTTPS request as the `apikey`\n    request\
  \ header. Quoted verbatim from the published API description: \"To use our API you\n    must be issued an API key. Instructions: For all HTTPS requests you will need to pass in\n    your API key as part of the header: `apikey: {API_KEY}`\".\n  issuance: manual — keys are issued by Aquabyte to existing customers; there is no public\n    self-service signup for API credentials.\n  sources:\n  - https://api.aquabyte.ai/openapi.json (info.description)\n  applies_to: all operations\nx-evidence:\n- fetched: '2026-08-06'\n  url: https://api.aquabyte.ai/openapi.json\n  http_status: 200\n  content_type: application/json\n  note: OpenAPI 3.1.0, 19 operations, no securitySchemes object\n- fetched: '2026-08-06'\n  url: https://api.aquabyte.ai/v3/sites\n  http_status: 401\n  note: unauthenticated request to a documented operation is rejected, confirming the key\n    requirement is enforced\n- fetched: '2026-08-06'\n  url: https://api.aquabyte.ai/v3/docs\n  http_status: 200\n  content_type: text/html\n\
  \  note: public ReDoc rendering of the same specification\ngaps:\n- No `components.securitySchemes` in the OpenAPI, so no machine-readable auth contract.\n- No OAuth 2.0 or OpenID Connect surface; no scopes, so `scopes/` is not applicable.\n- No `/.well-known/openid-configuration` or `/.well-known/oauth-authorization-server`\n  (both probed, both 404 on api.aquabyte.ai).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aquabyte/refs/heads/main/authentication/aquabyte-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Aquaculture
- Fish Farming
- Computer Vision
- Machine Learning
- Biomass Estimation
- Sea Lice
- Fish Welfare
- Environmental Monitoring
- Agriculture Technology
- Norway
- Salmon
- Data
---
