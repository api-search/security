---
api_key_in: []
api_specs:
- filename: university-of-sheffield-sheffield-solar-api-openapi.yml
  format: yaml
  label: Sheffield Solar API
  slug: sheffield-solar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-sheffield/refs/heads/main/openapi/university-of-sheffield-sheffield-solar-api-openapi.yml
auth_types:
- oauth2
- apiKey
- http
- saml2
description: ''
kind: authentication
layout: security
method: derived
name: University Of Sheffield Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Sheffield secures its APIs with oauth2, apiKey, http, and saml2 across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: University of Sheffield
provider_slug: university-of-sheffield
scheme_count: 5
schemes:
- api: Sheffield Solar API
  flows:
  - flow: password
    scopes: 0
    tokenUrl: https://api.solar.sheffield.ac.uk/auth/jwt/login
  name: OAuth2PasswordBearer
  note: Declared in the institution's published OpenAPI with an empty scopes object. Guards the PV_Forecast, /users and /admin operations, not the open PV_Live reads.
  source: https://api.solar.sheffield.ac.uk/openapi.json
  type: oauth2
- api: Sheffield Solar API
  in: cookie
  name: APIKeyCookie
  note: Browser session cookie for the Sheffield Solar web UI.
  parameter: ssapi_session
  source: https://api.solar.sheffield.ac.uk/openapi.json
  type: apiKey
- api: Sheffield Solar API
  name: HTTPBasic
  scheme: basic
  source: https://api.solar.sheffield.ac.uk/openapi.json
  type: http
- api: Sheffield Solar API
  in: header
  method: probed
  name: X-User-Id
  note: NOT declared in the published OpenAPI. Enforced at runtime on PV_Forecast endpoints and discovered by live probe — a 401 body naming the header. Recorded as an undocumented-but-real access control.
  parameter: X-User-Id
  source: https://api.solar.sheffield.ac.uk/pvforecast/api/v4/gsp/0
  type: apiKey
- api: Institutional identity federation
  bindings:
  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST
  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST-SimpleSign
  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect
  - urn:oasis:names:tc:SAML:2.0:bindings:SOAP
  entity_id: https://idp.shef.ac.uk/shibboleth
  metadata: https://idp.shef.ac.uk/idp/shibboleth
  method: probed
  name: Shibboleth IdP (SAML 2.0)
  note: Institution-operated Shibboleth identity provider. This is how a University of Sheffield affiliate authenticates into every vendor-tenanted service the institution buys, and it is the one access surface here that is unambiguously the institution's own engineering.
  source: https://idp.shef.ac.uk/idp/shibboleth
  type: saml2
slug: university-of-sheffield-authentication
source_filename: university-of-sheffield-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\ngenerated: '2026-08-30'\nmethod: derived\nsource: openapi/university-of-sheffield-sheffield-solar-api-openapi.yml\nprobed:\n  - url: https://api.solar.sheffield.ac.uk/pvlive/api/v4/gsp/0\n    status: 200\n    note: keyless\n  - url: https://api.solar.sheffield.ac.uk/pvforecast/api/v4/gsp/0\n    status: 401\n    note: identifier required\n  - url: https://idp.shef.ac.uk/idp/shibboleth\n    status: 200\n    note: institutional SAML 2.0 identity provider metadata\nprovider: University of Sheffield\nx-operator: institution\nsummary:\n  types:\n    - oauth2\n    - apiKey\n    - http\n    - saml2\n  public_read_without_credentials: true\nschemes:\n  - name: OAuth2PasswordBearer\n    api: Sheffield Solar API\n    type: oauth2\n    flows:\n      - flow: password\n        tokenUrl: https://api.solar.sheffield.ac.uk/auth/jwt/login\n        scopes: 0\n    note: >-\n      Declared in the institution's published OpenAPI with an empty scopes object.\n      Guards the PV_Forecast, /users\
  \ and /admin operations, not the open PV_Live reads.\n    source: https://api.solar.sheffield.ac.uk/openapi.json\n  - name: APIKeyCookie\n    api: Sheffield Solar API\n    type: apiKey\n    in: cookie\n    parameter: ssapi_session\n    note: Browser session cookie for the Sheffield Solar web UI.\n    source: https://api.solar.sheffield.ac.uk/openapi.json\n  - name: HTTPBasic\n    api: Sheffield Solar API\n    type: http\n    scheme: basic\n    source: https://api.solar.sheffield.ac.uk/openapi.json\n  - name: X-User-Id\n    api: Sheffield Solar API\n    type: apiKey\n    in: header\n    parameter: X-User-Id\n    note: >-\n      NOT declared in the published OpenAPI. Enforced at runtime on PV_Forecast\n      endpoints and discovered by live probe — a 401 body naming the header.\n      Recorded as an undocumented-but-real access control.\n    method: probed\n    source: https://api.solar.sheffield.ac.uk/pvforecast/api/v4/gsp/0\n  - name: Shibboleth IdP (SAML 2.0)\n    api: Institutional identity\
  \ federation\n    type: saml2\n    entity_id: https://idp.shef.ac.uk/shibboleth\n    metadata: https://idp.shef.ac.uk/idp/shibboleth\n    bindings:\n      - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n      - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST-SimpleSign\n      - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n      - urn:oasis:names:tc:SAML:2.0:bindings:SOAP\n    note: >-\n      Institution-operated Shibboleth identity provider. This is how a University\n      of Sheffield affiliate authenticates into every vendor-tenanted service the\n      institution buys, and it is the one access surface here that is unambiguously\n      the institution's own engineering.\n    method: probed\n    source: https://idp.shef.ac.uk/idp/shibboleth\nnotes: >-\n  The University of Sheffield operates no central API gateway, no developer-key\n  issuance and no self-service developer portal. Access is either fully open\n  (PV_Live), gated by a per-service registration (PV_Forecast), or gated\
  \ by\n  institutional SSO through the Shibboleth IdP.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-sheffield/refs/heads/main/authentication/university-of-sheffield-authentication.yml
summary_line: oauth2/apiKey/http/saml2 · 5 schemes
tags:
- University
- Higher Education
- Education
- United Kingdom
- Russell Group
- Research Data
- Open Access
- OAI-PMH
- Identity Federation
- Solar Energy
- Energy Data
- Research Computing
---
