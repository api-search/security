---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Aperia Technologies Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aperia Technologies secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Aperia Technologies
provider_slug: aperia-technologies
scheme_count: 1
schemes:
- description: 'HTTP Basic authentication (RFC 7617). The documentation instructs partners to send "Authorization: Basic <Base64_encoded_string>", where the token is the Base64 encoding of "email:password" — the same Halo Connect portal account credentials used to sign in at haloconnect.aperiatech.com. There is no separate API key, no token exchange, and no documented rotation or expiry.'
  in: header
  name: BasicAuth
  parameter: Authorization
  scheme: basic
  sources:
  - https://aperiatech.com/wp-content/uploads/2024/03/Halo-Connect-API-Documentation-v0.6.pdf
  type: http
slug: aperia-technologies-authentication
source_filename: aperia-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: https://aperiatech.com/wp-content/uploads/2024/03/Halo-Connect-API-Documentation-v0.6.pdf\ndocs: https://aperiatech.com/wp-content/uploads/2024/03/Halo-Connect-API-Documentation-v0.6.pdf\nnote: >-\n  Aperia publishes no OpenAPI, so this profile is read from the published PDF API reference\n  (\"Halo Connect API Documentation v0.6\", revised 2021-04-16) and corroborated by live probes\n  of the Halo Connect API gateway. Only the scheme is recorded; no credential values appear\n  in the source document beyond an illustrative Base64 sample.\nsummary:\n  types:\n  - http\n  http_schemes:\n  - basic\n  api_key_in: []\n  oauth2_flows: []\n  self_service_signup: false\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  in: header\n  parameter: Authorization\n  description: >-\n    HTTP Basic authentication (RFC 7617). The documentation instructs partners to send\n    \"Authorization: Basic <Base64_encoded_string>\", where\
  \ the token is the Base64 encoding\n    of \"email:password\" — the same Halo Connect portal account credentials used to sign in\n    at haloconnect.aperiatech.com. There is no separate API key, no token exchange, and no\n    documented rotation or expiry.\n  sources:\n  - https://aperiatech.com/wp-content/uploads/2024/03/Halo-Connect-API-Documentation-v0.6.pdf\ncredential_provisioning:\n  self_service: false\n  mechanism: >-\n    Halo Connect fleet accounts are created by an Aperia Technologies administrator; users\n    are invited by email and set a password. The same account credentials are what the\n    Partner API consumes, so API access follows portal provisioning rather than a developer\n    signup.\n  source: https://aperiatech.com/training/halo-connect-portal-training/\nobservations:\n- observed: '2026-08-06'\n  url: https://haloconnect.aperiatech.com/api/partner/v1/vehicles\n  http_status: 401\n  body: '{\"errorType\":\"UNAUTHORIZED\",\"errorMessage\":\"Unauthorized\"}'\n  note:\
  \ >-\n    No WWW-Authenticate challenge header is returned with the 401, so the Basic scheme is\n    not advertised at the wire level — it is only documented in the PDF. The same 401 is\n    returned for unrouted /api/* paths, so a 401 does not confirm an individual endpoint.\n- observed: '2026-08-06'\n  url: https://haloconnect.aperiatech.com/api/v1/health\n  http_status: 200\n  body: '{\"status\":\"UP\"}'\n  note: The health endpoint is the one documented operation reachable anonymously.\ngaps:\n- No OAuth 2.0 or OpenID Connect; long-lived user credentials are sent on every request.\n- No documented key rotation, expiry, scoping or least-privilege model for partner access.\n- No /.well-known/openid-configuration or /.well-known/oauth-authorization-server on any host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aperia-technologies/refs/heads/main/authentication/aperia-technologies-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Tire Management
- Fleet Management
- Telematics
- Transportation
- Trucking
- Automatic Tire Inflation
- Predictive Maintenance
- IoT
- Connected Vehicle
---
