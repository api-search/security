---
api_key_in:
- header
- body
api_specs:
- filename: novicap-openapi.yml
  format: yaml
  label: Novicap API
  slug: novicap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novicap/refs/heads/main/openapi/novicap-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Novicap Authentication
name_suffix: Authentication
oauth_flows: []
overview: Novicap secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Novicap
provider_slug: novicap
scheme_count: 2
schemes:
- description: 'API key generated from the Novicap user profile, sent as "Authorization: Bearer {api_key}". The key may alternatively be provided as an "api_key" field inside the JSON request payload.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/novicap-openapi.yml
  type: http
- available_on_request: true
  description: OAuth 2.0 is documented as available on request; scopes/flows are not published.
  name: oauth2
  type: oauth2
slug: novicap-authentication
source_filename: novicap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developer.novicap.com/#authentication\ndocs: https://developer.novicap.com/#authentication\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  oauth2_flows: []\n  api_key_in: [header, body]\n  product_scoped: true\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: >-\n      API key generated from the Novicap user profile, sent as\n      \"Authorization: Bearer {api_key}\". The key may alternatively be provided as\n      an \"api_key\" field inside the JSON request payload.\n    sources: [openapi/novicap-openapi.yml]\n  - name: oauth2\n    type: oauth2\n    description: OAuth 2.0 is documented as available on request; scopes/flows are not published.\n    available_on_request: true\nrequirements:\n  - Every request must include a product_id (query parameter or JSON payload field).\n  - Endpoint availability depends on account configuration; a 403 means the endpoint is not\
  \ enabled for the account (contact support@novicap.com).\nnotes: >-\n  Derived from the published API Reference. No OpenAPI is published by the\n  provider; the securityScheme is transcribed from the docs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/novicap/refs/heads/main/authentication/novicap-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Financial Services
- Fintech
- Working Capital
- Invoice Finance
- Supply Chain Finance
- Dynamic Discounting
- Confirming
- Reverse Factoring
- Spain
---
