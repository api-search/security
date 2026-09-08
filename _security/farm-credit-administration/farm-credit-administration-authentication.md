---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Farm Credit Administration Authentication
name_suffix: Authentication
oauth_flows: []
overview: Farm Credit Administration declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Farm Credit Administration
provider_slug: farm-credit-administration
scheme_count: 2
schemes:
- applies_to:
  - GET /arcgis/rest/services
  - GET /arcgis/rest/services/FCA
  - GET /arcgis/rest/services/FCA/{service}/MapServer
  - GET /arcgis/rest/services/FCA/{service}/MapServer/{layerId}
  - GET /arcgis/rest/services/FCA/{service}/MapServer/{layerId}/query
  evidence: https://wgis.fca.gov/arcgis/rest/services/FCA/hq/MapServer/0/query?where=1=1&returnCountOnly=true&f=json returned {"count":55} with no Authorization header and no token parameter.
  id: anonymous
  type: none
  verified: probed
- id: arcgis-token
  required_for_public_read: false
  scope_note: Reported by the server itself in /arcgis/rest/info as authInfo.isTokenBasedSecurity=true, tokenServicesUrl=https://wgis.fca.gov/arcgis/tokens/, shortLivedTokenValidity=60. This governs administrative and secured services; the three FCA folder services are open.
  short_lived_token_validity_minutes: 60
  style: query parameter or header (Esri ArcGIS Server token)
  token_service: https://wgis.fca.gov/arcgis/tokens/
  type: token
slug: farm-credit-administration-authentication
source_filename: farm-credit-administration-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: >-\n  https://wgis.fca.gov/arcgis/rest/info?f=json (fetched 2026-09-07, HTTP 200) plus anonymous\n  request/response observation against the FCA map services.\nsummary: >-\n  The public FCA map services require NO credential. Every service definition, layer definition and\n  /query call in arcgis/ and examples/ was made anonymously and returned 200. The ArcGIS Server\n  behind them does advertise token-based security for privileged operations, so the token service is\n  recorded here as the escalation path, not as a requirement for public reads.\nschemes:\n  - id: anonymous\n    type: none\n    applies_to:\n      - GET /arcgis/rest/services\n      - GET /arcgis/rest/services/FCA\n      - GET /arcgis/rest/services/FCA/{service}/MapServer\n      - GET /arcgis/rest/services/FCA/{service}/MapServer/{layerId}\n      - GET /arcgis/rest/services/FCA/{service}/MapServer/{layerId}/query\n    verified: probed\n    evidence: >-\n      https://wgis.fca.gov/arcgis/rest/services/FCA/hq/MapServer/0/query?where=1=1&returnCountOnly=true&f=json\n\
  \      returned {\"count\":55} with no Authorization header and no token parameter.\n  - id: arcgis-token\n    type: token\n    style: query parameter or header (Esri ArcGIS Server token)\n    token_service: https://wgis.fca.gov/arcgis/tokens/\n    short_lived_token_validity_minutes: 60\n    required_for_public_read: false\n    scope_note: >-\n      Reported by the server itself in /arcgis/rest/info as\n      authInfo.isTokenBasedSecurity=true, tokenServicesUrl=https://wgis.fca.gov/arcgis/tokens/,\n      shortLivedTokenValidity=60. This governs administrative and secured services; the three FCA\n      folder services are open.\noauth2: false\nopenid_connect: false\nmutual_tls: false\napi_keys: false\ndocs: null\ndocs_note: >-\n  FCA publishes no authentication documentation of any kind for this surface, because it publishes no\n  developer documentation of any kind for it. The auth model above was established by probing, not by\n  reading. The generic protocol reference is Esri's (ArcGIS\
  \ REST API), not FCA's.\ngaps:\n  - No developer portal, API reference, or getting-started page names these endpoints.\n  - No /.well-known/oauth-authorization-server or openid-configuration on any FCA host.\n  - No rate-limit, quota or terms-of-use statement attached to the anonymous read surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/farm-credit-administration/refs/heads/main/authentication/farm-credit-administration-authentication.yml
summary_line: 2 schemes
tags:
- Agriculture
- Farms
- Federal-Government
- Finance
- Regulations
- Geospatial
- Open-Data
- Banking
- Lending
- Government
---
