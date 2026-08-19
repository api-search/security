---
api_key_in:
- header
auth_types:
- ocpi-token
description: Electra has no OpenAPI, so this profile is not derived from securitySchemes — it is what the live surface actually answered. The single authenticated API Electra runs is its OCPI Charge Point Operator interface, and it uses OCPI's own bilateral Token scheme. There is no OAuth 2, no OpenID Connect, no self-service API key, no developer signup and no sandbox credential anywhere in Electra's public surface.
kind: authentication
layout: security
method: probed
name: Go Electra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Electra secures its APIs with ocpi-token across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Electra
provider_slug: go-electra
scheme_count: 1
schemes:
- applies_to: Every OCPI module endpoint under https://ocpi.go-electra.com/ocpi/cpo/2.1.1 and /2.2.1 (cdrs, commands, locations, sessions, tariffs, tokens).
  evidence:
  - body: 'Token: Access denied.'
    fetched: '2026-08-17'
    http_status: 401
    response_header: 'WWW-Authenticate: Token realm="Application"'
    url: https://ocpi.go-electra.com/ocpi/cpo/2.2.1/locations
  - body: 'Token: Access denied.'
    fetched: '2026-08-17'
    http_status: 401
    response_header: 'WWW-Authenticate: Token realm="Application"'
    url: https://ocpi.go-electra.com/ocpi/cpo/2.1.1/locations
  - body: 'Token: Access denied.'
    fetched: '2026-08-17'
    http_status: 401
    response_header: 'WWW-Authenticate: Token realm="Application"'
    url: https://ocpi.go-electra.com/ocpi/cpo/2.2.1/tariffs
  in: header
  name: OCPI Token
  onboarding: Bilateral. A roaming partner and Electra exchange OCPI credentials tokens through the credentials module; no public registration flow exists.
  parameter: Authorization
  realm: Application
  scheme: Token
  type: http
slug: go-electra-authentication
source_filename: go-electra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: >-\n  Anonymous probes of https://ocpi.go-electra.com/ocpi/cpo/* on 2026-08-17\n  (response headers and bodies), plus /.well-known/openid-configuration,\n  /.well-known/oauth-authorization-server and\n  /.well-known/oauth-protected-resource on go-electra.com, app.go-electra.com,\n  backend.go-electra.com and ocpi.go-electra.com.\ndescription: >-\n  Electra has no OpenAPI, so this profile is not derived from securitySchemes —\n  it is what the live surface actually answered. The single authenticated API\n  Electra runs is its OCPI Charge Point Operator interface, and it uses OCPI's\n  own bilateral Token scheme. There is no OAuth 2, no OpenID Connect, no\n  self-service API key, no developer signup and no sandbox credential anywhere\n  in Electra's public surface.\nsummary:\n  types: [ocpi-token]\n  api_key_in: [header]\n  oauth2_flows: []\n  self_service: false\n  note: >-\n    OCPI Token is an HTTP Authorization scheme with\
  \ the literal auth-scheme name\n    `Token` (Authorization: Token <credential>), exchanged bilaterally through\n    the OCPI credentials module after a commercial roaming agreement. It is not\n    an apiKey, http-bearer, oauth2 or openIdConnect scheme in OpenAPI terms,\n    which is why no standard securityScheme name is asserted here.\nschemes:\n- name: OCPI Token\n  type: http\n  scheme: Token\n  in: header\n  parameter: Authorization\n  realm: Application\n  applies_to: >-\n    Every OCPI module endpoint under https://ocpi.go-electra.com/ocpi/cpo/2.1.1\n    and /2.2.1 (cdrs, commands, locations, sessions, tariffs, tokens).\n  onboarding: >-\n    Bilateral. A roaming partner and Electra exchange OCPI credentials tokens\n    through the credentials module; no public registration flow exists.\n  evidence:\n  - url: https://ocpi.go-electra.com/ocpi/cpo/2.2.1/locations\n    http_status: 401\n    response_header: 'WWW-Authenticate: Token realm=\"Application\"'\n    body: 'Token: Access denied.'\n\
  \    fetched: '2026-08-17'\n  - url: https://ocpi.go-electra.com/ocpi/cpo/2.1.1/locations\n    http_status: 401\n    response_header: 'WWW-Authenticate: Token realm=\"Application\"'\n    body: 'Token: Access denied.'\n    fetched: '2026-08-17'\n  - url: https://ocpi.go-electra.com/ocpi/cpo/2.2.1/tariffs\n    http_status: 401\n    response_header: 'WWW-Authenticate: Token realm=\"Application\"'\n    body: 'Token: Access denied.'\n    fetched: '2026-08-17'\nunauthenticated_surface:\n- url: https://ocpi.go-electra.com/ocpi/cpo/versions\n  http_status: 200\n  note: Version negotiation is deliberately open — no token required.\n- url: https://ocpi.go-electra.com/ocpi/cpo/2.1.1\n  http_status: 200\n  note: Version-detail endpoint inventory is open.\n- url: https://ocpi.go-electra.com/ocpi/cpo/2.2.1\n  http_status: 200\n  note: Version-detail endpoint inventory is open.\nabsent:\n- scheme: oauth2\n  evidence: >-\n    /.well-known/oauth-authorization-server and\n    /.well-known/oauth-protected-resource\
  \ returned 404 on go-electra.com,\n    backend.go-electra.com and ocpi.go-electra.com, and an HTML SPA shell (not a\n    document) on app.go-electra.com. No OAuth is documented anywhere.\n- scheme: openIdConnect\n  evidence: >-\n    /.well-known/openid-configuration returned 404 on go-electra.com,\n    backend.go-electra.com and ocpi.go-electra.com; app.go-electra.com answers\n    200 with the same HTML SPA shell it serves for every path, which is not a\n    discovery document.\n- scheme: apiKey\n  evidence: >-\n    No developer portal, no key-issuance page and no API documentation exist on\n    any Electra host; the only key-shaped credential Electra publishes is a\n    consumer promo code.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/go-electra/refs/heads/main/authentication/go-electra-authentication.yml
summary_line: ocpi-token · 1 scheme
tags:
- Company
- Climate Tech
- EV Charging
- Energy
- Mobility
- OCPI
- Roaming
- Charge Point Operator
- Electric Vehicles
- Fast Charging
- Charging Sessions
- Tariffs
- Electrification
- France
- Europe
---
