---
api_key_in: []
api_specs:
- filename: landcor-property-api-openapi.json
  format: json
  label: Landcor Property API
  slug: landcor-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landcor/refs/heads/main/openapi/landcor-property-api-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Landcor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Landcor Data secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Landcor Data
provider_slug: landcor
scheme_count: 1
schemes:
- applies_to: 11 of 12 operations
  bearer_format: null
  header: 'Authorization: Bearer <token>'
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/landcor-property-api-openapi.json
  type: http
  unauthenticated_operations:
  - health_check_health_get
slug: landcor-authentication
source_filename: landcor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: derived\nsource: openapi/landcor-property-api-openapi.json\ndocs: https://api.landcor.com/docs\ndocs_note: >-\n  The only \"auth documentation\" Landcor publishes is the Authorize dialog in the Swagger UI\n  render of its own spec. There is no auth page, no developer portal and no key-issuance route\n  anywhere on landcor.com — verified against the site's full Yoast sitemap index on 2026-07-26.\n  method stays `derived` because nothing was harvested from a docs page.\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  bearer_format: null\n  header: 'Authorization: Bearer <token>'\n  sources:\n  - openapi/landcor-property-api-openapi.json\n  applies_to: 11 of 12 operations\n  unauthenticated_operations:\n  - health_check_health_get\naccess:\n  issuance: not-published\n  self_serve: false\n  detail: >-\n    This is the defining finding\
  \ for Landcor. The contract is anonymously readable — the OpenAPI,\n    Swagger UI and ReDoc all return HTTP 200 without credentials — but the token is not\n    obtainable through any published route. No developer portal, no API programme page, no key\n    request form, no partner page, no data-licensing page, no API pricing and no API terms exist\n    on landcor.com, and the marketing site never references api.landcor.com. The self-serve\n    account at https://store.landcor.com/user/user_add.aspx buys individual reports through the\n    web store; it is not an API credential. Access requires a direct commercial arrangement\n    (1-866-LANDCOR, https://www.landcor.com/contact/).\n  binding_terms: https://www.landcor.com/acceptable-use/\nevidence:\n- probe: GET https://api.landcor.com/property/search\n  date: '2026-07-26'\n  status: 401\n  body: '{\"detail\":\"Missing token\"}'\n  headers_observed: [Content-Length, Content-Type, Date, 'Server: uvicorn']\n  note: No WWW-Authenticate challenge\
  \ header was returned, which RFC 6750 expects on a 401 from a bearer-protected resource.\n- probe: GET https://api.landcor.com/address/autocomplete?q=main\n  date: '2026-07-26'\n  status: 401\n  body: '{\"detail\":\"Missing token\"}'\n- probe: GET https://api.landcor.com/valuationRange/123456789\n  date: '2026-07-26'\n  status: 401\n  body: '{\"detail\":\"Missing token\"}'\n- probe: GET https://api.landcor.com/health\n  date: '2026-07-26'\n  status: 200\n  body: '{\"status\":\"ok\"}'\n  note: The single operation callable anonymously.\n- probe: GET https://api.landcor.com/.well-known/oauth-authorization-server\n  date: '2026-07-26'\n  status: 404\n  note: >-\n    Also 404 for /.well-known/oauth-protected-resource and /.well-known/openid-configuration —\n    the bearer token is opaque and out-of-band, with no discoverable issuer. See\n    well-known/landcor-well-known.yml.\ntoken_properties:\n  format: unpublished\n  expiry: unpublished\n  refresh: unpublished\n  scopes: none\n  scopes_detail:\
  \ >-\n    No OAuth scheme and no scope surface, so scopes/ is intentionally absent — a single bearer\n    token carries whatever entitlement the commercial agreement grants, with nothing expressed in\n    the contract.\ncross_references:\n  conventions: conventions/landcor-conventions.yml\n  errors: errors/landcor-problem-types.yml\n  conformance: conformance/landcor-conformance.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/landcor/refs/heads/main/authentication/landcor-authentication.yml
summary_line: http · 1 scheme
tags:
- Real-Estate
- Canada
- Valuation
- AVM
- Property Records
- Title
- Land Registry
- Mortgage
- PropTech
- Property Data
---
