---
api_key_in: []
api_specs:
- filename: chargy-locations-api-openapi.yml
  format: yaml
  label: char.gy Locations API
  slug: chargy-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargy/refs/heads/main/openapi/chargy-locations-api-openapi.yml
- filename: chargy-tariffs-api-openapi.yml
  format: yaml
  label: char.gy Tariffs API
  slug: chargy-tariffs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargy/refs/heads/main/openapi/chargy-tariffs-api-openapi.yml
auth_types:
- none
- http
description: ''
kind: authentication
layout: security
method: probed
name: Chargy Authentication
name_suffix: Authentication
oauth_flows: []
overview: char.gy secures its APIs with none and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: char.gy
provider_slug: chargy
scheme_count: 2
schemes:
- applies_to: chargy:chargy-open-charge-point-data-api
  evidence: 'GET https://char.gy/open-ocpi/locations?limit=2 returned HTTP 200 with application/json and status_code 1000 to a request carrying no Authorization header, no cookie and no referer on 2026-07-27. The OpenAPI records this as an explicit empty `security: []` at both the document and operation level.'
  name: none
  self_service: not-applicable
  sources:
  - openapi/chargy-open-charge-point-data-openapi.yml
  surface: https://char.gy/open-ocpi
  type: none
- applies_to: chargy:chargy-ocpi-cpo-api
  credential_issuance: Partner-only. Credentials are exchanged through the OCPI credentials handshake following a commercial roaming agreement; the only published contact route is support@char.gy via https://char.gy/us/partners.
  documented: false
  evidence: 'GET https://char.gy/ocpi/cpo/versions and GET https://char.gy/ocpi/cpo/2.2.1/locations both returned HTTP 401 with the response header `www-authenticate: Token realm="OCPI"` and the body {"error":"HTTP Token: Access denied."} on 2026-07-27. This is the OCPI credentials-module token scheme (`Authorization: Token <credential>`), not OAuth 2.0.'
  in: header
  name: OCPI Token
  parameter_name: Authorization
  realm: OCPI
  scheme: Token
  self_service: false
  sources:
  - probe
  surface: https://char.gy/ocpi/cpo
  type: http
slug: chargy-authentication
source_filename: chargy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: >-\n  Live anonymous HTTP probes of https://char.gy/open-ocpi/* and\n  https://char.gy/ocpi/cpo/*, 2026-07-27; char.gy help-centre article\n  77000576948\ndocs: https://help.char.gy/support/solutions/articles/77000576948-public-charge-point-regulations-2023\nsummary:\n  types: [none, http]\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    char.gy operates two authentication postures on one host. The statutory open\n    data feed has NO authentication of any kind, by design and by law —\n    regulation 10(5) of the Public Charge Point Regulations 2023 forbids\n    requiring agreement to terms and conditions for access to that data, and no\n    credential, cookie or referer was needed to receive HTTP 200. The commercial\n    OCPI CPO roaming interface requires an OCPI Token credential issued through\n    a partner credentials handshake. There is no OAuth 2.0 server, no OpenID\n    Connect discovery document, no API-key self-service\
  \ and no developer\n    registration anywhere on the domain — all five /.well-known/ discovery\n    probes returned 404.\nschemes:\n  - name: none\n    type: none\n    applies_to: chargy:chargy-open-charge-point-data-api\n    surface: https://char.gy/open-ocpi\n    sources: [openapi/chargy-open-charge-point-data-openapi.yml]\n    evidence: >-\n      GET https://char.gy/open-ocpi/locations?limit=2 returned HTTP 200 with\n      application/json and status_code 1000 to a request carrying no\n      Authorization header, no cookie and no referer on 2026-07-27. The OpenAPI\n      records this as an explicit empty `security: []` at both the document and\n      operation level.\n    self_service: not-applicable\n  - name: OCPI Token\n    type: http\n    scheme: Token\n    in: header\n    parameter_name: Authorization\n    applies_to: chargy:chargy-ocpi-cpo-api\n    surface: https://char.gy/ocpi/cpo\n    realm: OCPI\n    sources: [probe]\n    evidence: >-\n      GET https://char.gy/ocpi/cpo/versions\
  \ and\n      GET https://char.gy/ocpi/cpo/2.2.1/locations both returned HTTP 401 with\n      the response header `www-authenticate: Token realm=\"OCPI\"` and the body\n      {\"error\":\"HTTP Token: Access denied.\"} on 2026-07-27. This is the OCPI\n      credentials-module token scheme (`Authorization: Token <credential>`),\n      not OAuth 2.0.\n    credential_issuance: >-\n      Partner-only. Credentials are exchanged through the OCPI credentials\n      handshake following a commercial roaming agreement; the only published\n      contact route is support@char.gy via https://char.gy/us/partners.\n    self_service: false\n    documented: false\nabsent:\n  - oauth2: no authorization server; /.well-known/oauth-authorization-server 404\n  - openIdConnect: /.well-known/openid-configuration 404\n  - apiKey: no self-service API key issuance published anywhere on the domain\n  - mutualTLS: not observed\nconsumer_data_access: >-\n  There is no authenticated consumer-facing API. No surface exposes\
  \ an\n  individual driver's charging sessions, usage or billing data to that driver or\n  to a party acting on their behalf, because the United Kingdom has no energy\n  data-portability mandate equivalent to Australia's Consumer Data Right.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chargy/refs/heads/main/authentication/chargy-authentication.yml
summary_line: none/http · 2 schemes
tags:
- Energy
- United Kingdom
- EV Charging
- Electricity
- Utilities
- OCPI
- Charge Point Operator
- Open Data
- Roaming
- Tariffs
- Mobility
- Electrification
---
