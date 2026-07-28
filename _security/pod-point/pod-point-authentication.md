---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Pod Point Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pod Point secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Pod Point
provider_slug: pod-point
scheme_count: 3
schemes:
- api: pod-point:pod-point-ocpi-cpo-api
  description: OCPI 2.2.1 authenticates with an HTTP Authorization header carrying a Token A / Token B / Token C obtained through the /credentials module handshake. By design the handshake requires both parties to already hold each other's registration details, so there is no anonymous or self-service path to a token. Pod publishes no form, no email address, no partner API page and no criteria for obtaining one; in practice it means a commercial roaming or eMSP relationship.
  docs: https://github.com/ocpi/ocpi
  evidence:
  - body: '{"status_code":2000,"status_message":"Unauthorized"}'
    probe: GET https://ocpi.podenergy.com/ocpi/cpo/2.2.1/locations
    status: 401
  - probe: GET https://ocpi.podenergy.com/ocpi/cpo/2.2.1/tariffs
    status: 401
  - probe: GET https://ocpi.podenergy.com/ocpi/cpo/2.2.1/sessions
    status: 401
  - probe: GET https://ocpi.podenergy.com/ocpi/cpo/2.2.1/cdrs
    status: 401
  - probe: GET https://ocpi.podenergy.com/ocpi/cpo/2.2.1/credentials
    status: 401
  - note: Version negotiation is the only anonymous surface.
    probe: GET https://ocpi.podenergy.com/ocpi/cpo/versions
    status: 200
  format: 'Authorization: Token <base64-encoded credentials token>'
  in: header
  name: OCPI credentials token
  parameter_name: Authorization
  registration: bilateral
  scheme: Token
  self_service: false
  standard: OCPI 2.2.1, credentials module
  status: live
  type: http
- base_url: https://api.pod-point.com/v3/
  base_url_status: 403
  description: 'The retired Pod Point Network API v3 exchanged user credentials for an access token by POST to the `auth` endpoint, then sent `Authorization: <tokenType> <accessToken>` on subsequent calls. The SDK Client was additionally constructed with an accessKey and secretKey pair (Client(accessKey, secretKey, userAgent, domain, prefix)) and bundles crypto-js, indicating a request-signing layer on top of the bearer token.'
  in: header
  name: Pod Point Network API v3 bearer token
  note: Host decommissioned — returns S3 AccessDenied on every path. Recorded for lineage only.
  parameter_name: Authorization
  scheme: bearer
  source: '@pod-point/api3-js v6.4.2 lib/services/AuthenticationService.js'
  status: legacy
  type: http
- base_url: https://api.pod-point.com/v5/
  base_url_status: 403
  description: Same auth endpoint pattern as v3, against the /v5/ prefix. Host decommissioned.
  in: header
  name: Pod Point API v5 auth
  parameter_name: Authorization
  scheme: bearer
  source: '@pod-point/api5-js v1.2.0'
  status: legacy
  type: http
slug: pod-point-authentication
source_filename: pod-point-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  Live anonymous probes of https://ocpi.podenergy.com on 2026-07-27, the OCPI 2.2.1-d2\n  specification, and the first-party @pod-point/api3-js and @pod-point/api5-js SDK\n  sources.\nnote: >-\n  Derived without an OpenAPI, because Pod publishes none. The auth model for the one\n  live API was established from the wire: every OCPI data module answers HTTP 401 with\n  the OCPI status_code 2000 envelope to an anonymous caller, and no OIDC or OAuth\n  authorization-server metadata exists on any Pod host. The legacy schemes are read\n  out of Pod's own published SDK source, not guessed.\nsummary:\n  types: [http]\n  api_key_in: [header]\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\n  anonymous_surface: >-\n    OCPI version negotiation only (GET /ocpi/cpo/versions and GET /ocpi/cpo/2.2.1).\n    Nothing that carries data is reachable anonymously.\nschemes:\n- name: OCPI credentials token\n  api: pod-point:pod-point-ocpi-cpo-api\n\
  \  type: http\n  scheme: Token\n  in: header\n  parameter_name: Authorization\n  format: \"Authorization: Token <base64-encoded credentials token>\"\n  status: live\n  standard: OCPI 2.2.1, credentials module\n  registration: bilateral\n  self_service: false\n  docs: https://github.com/ocpi/ocpi\n  description: >-\n    OCPI 2.2.1 authenticates with an HTTP Authorization header carrying a Token A /\n    Token B / Token C obtained through the /credentials module handshake. By design\n    the handshake requires both parties to already hold each other's registration\n    details, so there is no anonymous or self-service path to a token. Pod publishes\n    no form, no email address, no partner API page and no criteria for obtaining one;\n    in practice it means a commercial roaming or eMSP relationship.\n  evidence:\n  - probe: GET https://ocpi.podenergy.com/ocpi/cpo/2.2.1/locations\n    status: 401\n    body: '{\"status_code\":2000,\"status_message\":\"Unauthorized\"}'\n  - probe: GET https://ocpi.podenergy.com/ocpi/cpo/2.2.1/tariffs\n\
  \    status: 401\n  - probe: GET https://ocpi.podenergy.com/ocpi/cpo/2.2.1/sessions\n    status: 401\n  - probe: GET https://ocpi.podenergy.com/ocpi/cpo/2.2.1/cdrs\n    status: 401\n  - probe: GET https://ocpi.podenergy.com/ocpi/cpo/2.2.1/credentials\n    status: 401\n  - probe: GET https://ocpi.podenergy.com/ocpi/cpo/versions\n    status: 200\n    note: Version negotiation is the only anonymous surface.\n- name: Pod Point Network API v3 bearer token\n  type: http\n  scheme: bearer\n  in: header\n  parameter_name: Authorization\n  status: legacy\n  source: \"@pod-point/api3-js v6.4.2 lib/services/AuthenticationService.js\"\n  description: >-\n    The retired Pod Point Network API v3 exchanged user credentials for an access\n    token by POST to the `auth` endpoint, then sent `Authorization: <tokenType>\n    <accessToken>` on subsequent calls. The SDK Client was additionally constructed\n    with an accessKey and secretKey pair (Client(accessKey, secretKey, userAgent,\n    domain, prefix))\
  \ and bundles crypto-js, indicating a request-signing layer on top\n    of the bearer token.\n  base_url: https://api.pod-point.com/v3/\n  base_url_status: 403\n  note: Host decommissioned — returns S3 AccessDenied on every path. Recorded for lineage only.\n- name: Pod Point API v5 auth\n  type: http\n  scheme: bearer\n  in: header\n  parameter_name: Authorization\n  status: legacy\n  source: \"@pod-point/api5-js v1.2.0\"\n  base_url: https://api.pod-point.com/v5/\n  base_url_status: 403\n  description: Same auth endpoint pattern as v3, against the /v5/ prefix. Host decommissioned.\nnot_present:\n- scheme: oauth2\n  evidence: >-\n    No /.well-known/oauth-authorization-server on podenergy.com, ocpi.podenergy.com or\n    mobile-api.pod-point.com (all 404).\n- scheme: openIdConnect\n  evidence: >-\n    No /.well-known/openid-configuration on any Pod host — podenergy.com 404,\n    ocpi.podenergy.com 404, mobile-api.pod-point.com 404, api.pod-point.com 403.\n- scheme: apiKey self-service\n\
  \  evidence: >-\n    No developer portal, no signup, no key issuance page. developer., developers.,\n    docs. and data. do not resolve on either pod-point.com or podenergy.com.\n- scheme: mutualTLS\n  evidence: Not advertised; OCPI 2.2.1 does not require it and no client-cert challenge was observed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pod-point/refs/heads/main/authentication/pod-point-authentication.yml
summary_line: http · 3 schemes
tags:
- Energy
- United Kingdom
- EV Charging
- Electric Vehicles
- Utilities
- Electricity
- OCPI
- Charge Point Operator
- Smart Charging
- Grid
---
