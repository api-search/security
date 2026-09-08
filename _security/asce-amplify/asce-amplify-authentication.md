---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: asce-amplify-hazard-loads-openapi.yml
  format: yaml
  label: ASCE Hazard Tool API
  slug: hazard-tool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asce-amplify/refs/heads/main/openapi/asce-amplify-hazard-loads-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Asce Amplify Authentication
name_suffix: Authentication
oauth_flows: []
overview: ASCE Amplify secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ASCE Amplify
provider_slug: asce-amplify
scheme_count: 1
schemes:
- applies_to:
  - ASCE Hazard Tool API
  description: Every ASCE Hazard Loads API request authenticates with an API key passed as the `token` query parameter. Keys are issued per company at sign-up and are managed through the ASCE Hazard Tool Account Manager. ASCE publishes a sample key format on the documentation page (a UUID v4 string); it is a format illustration, not a working credential.
  in: query
  issuance: Issued to the company at the time of sign-up via the ASCE Hazard Tool Account Manager. Higher usage limits are arranged through the quote form.
  key_format: UUID v4 (as illustrated in the ASCE documentation)
  name: ApiKeyAuth
  parameter: token
  rotation: not documented
  sources:
  - openapi/asce-amplify-hazard-loads-openapi.yml
  - https://www.asce.org/publications-and-news/asce-hazard-tool/api
  type: apiKey
slug: asce-amplify-authentication
source_filename: asce-amplify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: https://www.asce.org/publications-and-news/asce-hazard-tool/api\ndocs: https://www.asce.org/publications-and-news/asce-hazard-tool/api\nspec_source: openapi/asce-amplify-hazard-loads-openapi.yml\nprovider: ASCE Amplify\nproviderId: asce-amplify\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - query\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: query\n    parameter: token\n    description: >-\n      Every ASCE Hazard Loads API request authenticates with an API key passed as\n      the `token` query parameter. Keys are issued per company at sign-up and are\n      managed through the ASCE Hazard Tool Account Manager. ASCE publishes a\n      sample key format on the documentation page (a UUID v4 string); it is a\n      format illustration, not a working credential.\n    key_format: UUID v4 (as illustrated in the ASCE documentation)\n    issuance:\
  \ >-\n      Issued to the company at the time of sign-up via the ASCE Hazard Tool\n      Account Manager. Higher usage limits are arranged through the quote form.\n    rotation: not documented\n    applies_to:\n      - ASCE Hazard Tool API\n    sources:\n      - openapi/asce-amplify-hazard-loads-openapi.yml\n      - https://www.asce.org/publications-and-news/asce-hazard-tool/api\nobserved:\n  - probe: GET https://api-hazard.asce.org/v1/wind\n    http_status: 401\n    body: '{\"code\":401,\"message\":\"Token required\"}'\n    fetched: '2026-09-07'\n    note: >-\n      Anonymous call to a live operation. The documentation page states code 500\n      for a missing or invalid key; the deployed API answers 401 with a JSON\n      envelope of {code, message}. Recorded as observed behavior, not a\n      contradiction we are asserting on ASCE's behalf.\nnotes:\n  - >-\n    The ASCE Hazard Loads API declares no OAuth2 or OpenID Connect scheme, so no\n    scopes/ artifact is applicable.\n  - >-\n\
  \    The separate ASCE GIS REST surface at gis.asce.org answers anonymously for the\n    published hazard services; /arcgis/rest/info reports\n    isTokenBasedSecurity: true with a token service at\n    https://gis.asce.org/arcgis/tokens/ for the secured/administrative surface.\n  - >-\n    The ASCE AMPLIFY web application (amplify.asce.org) authenticates humans over\n    OpenID Connect against the SAMS Sigma identity provider\n    (https://idp.sams-sigma.com, issuer confirmed in its published\n    /.well-known/openid-configuration). That is the application SSO, not an API\n    authentication path.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asce-amplify/refs/heads/main/authentication/asce-amplify-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Civil Engineering
- Hazard Data
- Engineering Standards
- Infrastructure
- Structural Engineering
- Geospatial
- Seismic
- Building Codes
- Standards Body
---
