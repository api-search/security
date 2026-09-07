---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aaravunmannedsystems-tile-server-openapi-original.json
  format: json
  label: Aereo Cloud Tile Server
  slug: aaravunmannedsystems-tile-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaravunmannedsystems/refs/heads/main/openapi/aaravunmannedsystems-tile-server-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Aaravunmannedsystems Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aarav Unmanned Systems (Aereo) secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Aarav Unmanned Systems (Aereo)
provider_slug: aaravunmannedsystems
scheme_count: 1
schemes:
- declared_in_openapi: false
  evidence:
  - 'Aereo Cloud client sends `Authorization: Bearer ${token}` on its backend calls (observed verbatim in the cloud.aereo.io production JS bundle).'
  - GET https://tiles.aereo.io/terrain/layer.json -> 401 unauthenticated
  - GET https://tiles.aereo.io/vector/1/1/1.pbf -> 401 unauthenticated
  - GET https://tiles.aereo.io/altitude -> 401 unauthenticated
  in: header
  method: probed
  name: bearerAuth
  parameter: Authorization
  scheme: bearer
  type: http
slug: aaravunmannedsystems-authentication
source_filename: aaravunmannedsystems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: >-\n  Live probes of https://tiles.aereo.io operations plus the Aereo Cloud SPA bundle\n  (https://cloud.aereo.io/assets/index-0BComw20.js), which names the auth scheme it sends.\nnote: >-\n  THE SPEC UNDER-DECLARES ITS OWN AUTH. openapi/aaravunmannedsystems-tile-server-openapi-original.json\n  declares NO components.securitySchemes and no security[] on any operation, yet every operation except\n  GET /ping returns HTTP 401 unauthenticated. The auth model below was established by probing, not by\n  reading the contract — an agent working from the published spec alone would believe the API is open.\n  This is a contract-quality gap worth reporting to the provider.\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: []\n  oauth2_flows: []\n  declared_in_spec: false\n  observed_by_probe: true\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  method: probed\n\
  \  declared_in_openapi: false\n  evidence:\n  - >-\n    Aereo Cloud client sends `Authorization: Bearer ${token}` on its backend calls\n    (observed verbatim in the cloud.aereo.io production JS bundle).\n  - GET https://tiles.aereo.io/terrain/layer.json -> 401 unauthenticated\n  - GET https://tiles.aereo.io/vector/1/1/1.pbf -> 401 unauthenticated\n  - GET https://tiles.aereo.io/altitude -> 401 unauthenticated\nidentity_providers:\n- name: Microsoft Entra ID (Azure AD)\n  protocol: OpenID Connect\n  method: probed\n  note: >-\n    The Aereo Cloud SPA embeds MSAL (@azure/msal-browser) with a fixed azureClientId and a\n    https://cloud.aereo.io/auth/microsoft-redirect callback against login.microsoftonline.com.\n    This is end-user SSO into the console, not a documented API authorization flow — no OAuth\n    authorization/token endpoint is published for third-party API clients.\n  evidence:\n  - https://login.microsoftonline.com/ referenced in the cloud.aereo.io bundle\n  - https://cloud.aereo.io/auth/microsoft-redirect\
  \ referenced in the cloud.aereo.io bundle\nunauthenticated_operations:\n- operation: ping_ping_get\n  path: /ping\n  note: Health check; returns {\"data\":\"pong\"} with no credential.\ngaps:\n- No securitySchemes in the published OpenAPI despite enforced bearer auth.\n- No documented token issuance endpoint, token lifetime, or scope model for API clients.\n- No /.well-known/openid-configuration or /.well-known/oauth-authorization-server on any aereo.io host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aaravunmannedsystems/refs/heads/main/authentication/aaravunmannedsystems-authentication.yml
summary_line: http · 1 scheme
tags:
- Drones
- UAV
- Geospatial
- Mapping
- Remote Sensing
- Surveying
- Mining
- Agriculture
- Satellite Imagery
- Analytics
- India
---
