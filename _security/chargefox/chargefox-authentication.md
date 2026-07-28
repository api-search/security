---
api_key_in: []
api_specs:
- filename: chargefox-fleets-api-openapi.json
  format: json
  label: Chargefox Fleets API
  slug: chargefox-fleets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargefox/refs/heads/main/openapi/chargefox-fleets-api-openapi.json
auth_types:
- http
- custom
description: Chargefox runs two different authentication models across two API surfaces, and neither is self-service. The Fleets API uses an opaque HTTP bearer token issued by Chargefox to fleet customers on request. The OCPI CPO API uses OCPI's own Token authorization scheme, established through the OCPI credentials handshake after a commercial roaming agreement. There is no OAuth, no OpenID Connect, no API-key console and no signup — probes of /.well-known/oauth-authorization-server, /.well-known/oauth-protected-resource and /.well-known/openid-configuration all returned 404 on 2026-07-27.
kind: authentication
layout: security
method: searched
name: Chargefox Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chargefox secures its APIs with http and custom across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Chargefox
provider_slug: chargefox
scheme_count: 2
schemes:
- api: chargefox:chargefox-fleets-api
  applied_to:
  - GET /api/fleets/v1/usage
  - GET /api/fleets/v1/sessions
  - GET /api/fleets/v1/vehicles
  - GET /api/fleets/v1/invoices
  docs: https://app.chargefox.com/developers/docs/getting_started
  example_request: 'curl --request GET --url ''https://app.chargefox.com/api/fleets/v1/usage'' --header ''Authorization: Bearer <token>'''
  expiry: undocumented
  format: Bearer <token>
  header: Authorization
  in: header
  issuance:
    contact: fleetsupport@chargefox.com
    process: Chargefox's getting-started page states that a fleet customer interested in using the API should speak to a team member or reach out via fleetsupport@chargefox.com. No developer portal signup, no key-management console and no sandbox key exist.
    self_service: false
  name: bearerAuth
  rotation: undocumented
  scheme: bearer
  scopes: none
  sources:
  - openapi/chargefox-fleets-api-openapi.json
  token_format: opaque
  type: http
- api: chargefox:chargefox-ocpi-cpo-api
  evidence: 'Anonymous GET of /ocpi/cpo/versions, /ocpi/cpo/2.1.1/, /ocpi/cpo/2.1.1/locations, /ocpi/cpo/2.2/, /ocpi/cpo/2.2.1/ and /ocpi/emsp/versions each returned HTTP 401 with the response header `WWW-Authenticate: Token realm="Application"`. Sibling paths /ocpi/, /ocpi/cpo/ and /ocpi/xyz/versions returned 404, confirming the 401 marks a real authenticated route rather than a blanket wall.'
  format: Token <credentials-token>
  header: Authorization
  in: header
  issuance:
    partners: https://www.chargefox.com/partners
    process: OCPI credentials are exchanged in the specification's own credentials module handshake once a roaming agreement is in place. Chargefox publishes roaming partner terms and conditions rather than a developer signup.
    self_service: false
    terms: https://www.chargefox.com/legal/roaming-partner-terms-and-conditions
  name: ocpiToken
  scheme: Token
  scopes: none
  sources:
  - live probe of https://app.chargefox.com/ocpi/cpo/* on 2026-07-27
  specification: https://github.com/ocpi/ocpi
  type: custom
slug: chargefox-authentication
source_filename: chargefox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: openapi/chargefox-fleets-api-openapi.json\ndocs: https://app.chargefox.com/developers/docs/getting_started\ndescription: >-\n  Chargefox runs two different authentication models across two API surfaces,\n  and neither is self-service. The Fleets API uses an opaque HTTP bearer token\n  issued by Chargefox to fleet customers on request. The OCPI CPO API uses\n  OCPI's own Token authorization scheme, established through the OCPI\n  credentials handshake after a commercial roaming agreement. There is no OAuth,\n  no OpenID Connect, no API-key console and no signup — probes of\n  /.well-known/oauth-authorization-server, /.well-known/oauth-protected-resource\n  and /.well-known/openid-configuration all returned 404 on 2026-07-27.\nsummary:\n  types:\n  - http\n  - custom\n  api_key_in: []\n  oauth2_flows: []\n  self_service: false\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  api: chargefox:chargefox-fleets-api\n\
  \  in: header\n  header: Authorization\n  format: 'Bearer <token>'\n  sources:\n  - openapi/chargefox-fleets-api-openapi.json\n  applied_to:\n  - GET /api/fleets/v1/usage\n  - GET /api/fleets/v1/sessions\n  - GET /api/fleets/v1/vehicles\n  - GET /api/fleets/v1/invoices\n  issuance:\n    self_service: false\n    process: >-\n      Chargefox's getting-started page states that a fleet customer interested\n      in using the API should speak to a team member or reach out via\n      fleetsupport@chargefox.com. No developer portal signup, no key-management\n      console and no sandbox key exist.\n    contact: fleetsupport@chargefox.com\n  token_format: opaque\n  rotation: undocumented\n  expiry: undocumented\n  scopes: none\n  docs: https://app.chargefox.com/developers/docs/getting_started\n  example_request: >-\n    curl --request GET --url\n    'https://app.chargefox.com/api/fleets/v1/usage' --header 'Authorization:\n    Bearer <token>'\n- name: ocpiToken\n  type: custom\n  scheme: Token\n\
  \  api: chargefox:chargefox-ocpi-cpo-api\n  in: header\n  header: Authorization\n  format: 'Token <credentials-token>'\n  sources:\n  - live probe of https://app.chargefox.com/ocpi/cpo/* on 2026-07-27\n  evidence: >-\n    Anonymous GET of /ocpi/cpo/versions, /ocpi/cpo/2.1.1/,\n    /ocpi/cpo/2.1.1/locations, /ocpi/cpo/2.2/, /ocpi/cpo/2.2.1/ and\n    /ocpi/emsp/versions each returned HTTP 401 with the response header\n    `WWW-Authenticate: Token realm=\"Application\"`. Sibling paths /ocpi/,\n    /ocpi/cpo/ and /ocpi/xyz/versions returned 404, confirming the 401 marks a\n    real authenticated route rather than a blanket wall.\n  issuance:\n    self_service: false\n    process: >-\n      OCPI credentials are exchanged in the specification's own credentials\n      module handshake once a roaming agreement is in place. Chargefox publishes\n      roaming partner terms and conditions rather than a developer signup.\n    terms: https://www.chargefox.com/legal/roaming-partner-terms-and-conditions\n\
  \    partners: https://www.chargefox.com/partners\n  specification: https://github.com/ocpi/ocpi\n  scopes: none\ndiscovery:\n  well_known_probed: well-known/chargefox-well-known.yml\n  oauth_authorization_server: 404\n  oauth_protected_resource: 404\n  openid_configuration: 404\n  security_txt: '403 (app.chargefox.com) / 404 (www.chargefox.com)'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chargefox/refs/heads/main/authentication/chargefox-authentication.yml
summary_line: http/custom · 2 schemes
tags:
- Energy
- Australia
- EV Charging
- Electricity
- Utilities
- OCPI
- Charge Point Operator
- Roaming
- Fleets
- Mobility
- Charging Sessions
- Electrification
---
