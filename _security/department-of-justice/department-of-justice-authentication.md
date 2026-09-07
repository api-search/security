---
anonymous_access: true
api_key_in:
- header
- query
api_specs:
- filename: department-of-justice-foia-api-swagger.json
  format: json
  label: National FOIA Portal API
  slug: foia-annual-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-justice/refs/heads/main/openapi/department-of-justice-foia-api-swagger.json
auth_types:
- apiKey
- none
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Department Of Justice Authentication
name_suffix: Authentication
oauth_flows: []
overview: Department of Justice secures its APIs with apiKey and none across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Department of Justice
provider_slug: department-of-justice
scheme_count: 2
schemes:
- alternates:
  - in: query
    note: Accepted by the gateway; the FOIA docs use it in their own curl examples.
    parameter: api_key
  - in: header
    note: api.data.gov also accepts the key as the HTTP basic-auth username with an empty password. Documented by the gateway, not by DOJ.
    parameter: Authorization
    scheme: basic
  applies_to: National FOIA Portal JSON:API (https://api.foia.gov/api)
  in: header
  issuer: api.data.gov (GSA)
  key_shape: 40-character opaque string
  missing_credential_response:
    body: '{"error":{"code":"API_KEY_MISSING","message":"No api_key was supplied. Get one at https://api.data.gov/signup/"}}'
    evidence: https://api.foia.gov/api/agency_components probed 2026-09-06
    status: 403
  name: APIKeyHeader
  parameter: X-API-Key
  shared_test_credential:
    note: 'The contract''s info.description publishes a working test api_key inline for the Swagger UI "Authorize" button, and api.data.gov publishes a shared DEMO_KEY. Both are heavily rate limited (DEMO_KEY: 30 requests per IP per hour, 50 per day). The literal value is not reproduced in this repository.'
    published: true
  signup: https://www.foia.gov/developer/#api-key-signup
  sources:
  - openapi/department-of-justice-foia-api-swagger.json
  - https://www.foia.gov/developer/
  - https://api.data.gov/docs/developer-manual/
  type: apiKey
- applies_to:
  - DOJ News API (https://www.justice.gov/api/v1)
  - BJS NCVS / NIBRS National Estimates (https://api.ojp.gov/bjsdataset/v1)
  - FARA e-File Registrant feed (https://efile.fara.gov/api/v1)
  - DOJ Open Data Catalog (https://www.justice.gov/data.json)
  evidence: Anonymous GETs returned 200 on 2026-09-06 for https://www.justice.gov/api/v1/press_releases.json?pagesize=1, https://api.ojp.gov/bjsdataset/v1/r32q-bdaw.json?$limit=1, https://efile.fara.gov/api/v1/Registrants/json/Active and https://www.justice.gov/data.json. No key, header or token of any kind is documented or required.
  name: None
  type: none
slug: department-of-justice-authentication
source_filename: department-of-justice-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nprovider: Department of Justice\nproviderId: department-of-justice\nsource: >-\n  Derived from openapi/department-of-justice-foia-api-swagger.json, then upgraded from the\n  provider's own auth documentation at https://www.foia.gov/developer/ and the gateway manual at\n  https://api.data.gov/docs/developer-manual/, and confirmed against live anonymous responses on\n  every DOJ API host on 2026-09-06.\ndocs: https://www.foia.gov/developer/\nsummary:\n  types: [apiKey, none]\n  api_key_in: [header, query]\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  note: >-\n    DOJ operates two auth postures side by side. Most of its public data is unauthenticated. Only\n    the National FOIA Portal requires a credential, and that credential is not issued by DOJ — it\n    is a shared federal api.data.gov key that works across every participating agency.\nschemes:\n  - name: APIKeyHeader\n    type: apiKey\n    in: header\n    parameter:\
  \ X-API-Key\n    applies_to: National FOIA Portal JSON:API (https://api.foia.gov/api)\n    issuer: api.data.gov (GSA)\n    signup: https://www.foia.gov/developer/#api-key-signup\n    key_shape: 40-character opaque string\n    alternates:\n      - in: query\n        parameter: api_key\n        note: 'Accepted by the gateway; the FOIA docs use it in their own curl examples.'\n      - in: header\n        parameter: Authorization\n        scheme: basic\n        note: >-\n          api.data.gov also accepts the key as the HTTP basic-auth username with an empty\n          password. Documented by the gateway, not by DOJ.\n    missing_credential_response:\n      status: 403\n      body: '{\"error\":{\"code\":\"API_KEY_MISSING\",\"message\":\"No api_key was supplied. Get one at https://api.data.gov/signup/\"}}'\n      evidence: 'https://api.foia.gov/api/agency_components probed 2026-09-06'\n    shared_test_credential:\n      published: true\n      note: >-\n        The contract's info.description\
  \ publishes a working test api_key inline for the Swagger UI\n        \"Authorize\" button, and api.data.gov publishes a shared DEMO_KEY. Both are heavily rate\n        limited (DEMO_KEY: 30 requests per IP per hour, 50 per day). The literal value is not\n        reproduced in this repository.\n    sources:\n      - openapi/department-of-justice-foia-api-swagger.json\n      - https://www.foia.gov/developer/\n      - https://api.data.gov/docs/developer-manual/\n  - name: None\n    type: none\n    applies_to:\n      - DOJ News API (https://www.justice.gov/api/v1)\n      - BJS NCVS / NIBRS National Estimates (https://api.ojp.gov/bjsdataset/v1)\n      - FARA e-File Registrant feed (https://efile.fara.gov/api/v1)\n      - DOJ Open Data Catalog (https://www.justice.gov/data.json)\n    evidence: >-\n      Anonymous GETs returned 200 on 2026-09-06 for\n      https://www.justice.gov/api/v1/press_releases.json?pagesize=1,\n      https://api.ojp.gov/bjsdataset/v1/r32q-bdaw.json?$limit=1,\n      https://efile.fara.gov/api/v1/Registrants/json/Active\
  \ and\n      https://www.justice.gov/data.json. No key, header or token of any kind is documented or\n      required.\nabsent:\n  - mechanism: OAuth 2.0\n    evidence: '/.well-known/oauth-authorization-server returned 404 on all eight probed hosts, 2026-09-06.'\n  - mechanism: OpenID Connect\n    evidence: '/.well-known/openid-configuration returned 404 on all eight probed hosts, 2026-09-06.'\n  - mechanism: Scopes / permissions\n    evidence: >-\n      No scope model exists. derive-oauth-scopes.py found no oauth2 securityScheme, and no DOJ\n      documentation describes permissions — the api.data.gov key is all-or-nothing across every\n      participating agency API.\n  - mechanism: mTLS\n    evidence: No client-certificate requirement documented on any surface.\ntransport_security:\n  https_enforced: true\n  hsts: true\n  note: >-\n    All four DOJ-operated hosts serve TLS 1.3 with HSTS. api.foia.gov returns\n    'strict-transport-security: max-age=31536000; includeSubDomains; preload'.\
  \ See\n    security/department-of-justice-domain-security.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/department-of-justice/refs/heads/main/authentication/department-of-justice-authentication.yml
summary_line: apiKey/none · 2 schemes
tags:
- Bureau of Justice Statistics
- Crime
- Federal-Government
- FOIA
- Justice
- News
- Open Data
- Press Releases
- Statistics
---
