---
api_key_in: []
auth_types:
- oauth2
- http
- none
description: ''
kind: authentication
layout: security
method: searched
name: Dexcare Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: DexCare secures its APIs with oauth2, http, and none across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: DexCare
provider_slug: dexcare
scheme_count: 3
schemes:
- bearerFormat: JWT
  description: JSON Web Token passed as a bearer token in the Authorization header for any endpoint that works with protected health information (PHI) or personally identifiable information (PII).
  header: Authorization
  in: header
  name: bearerJWT
  scheme: bearer
  sources:
  - https://developers.dexcarehealth.com/api/
  type: http
- description: OAuth 2.0 Authorization Code Grant flow used to obtain the JWT bearer token. Authorization and token endpoints are provided per health system via that system's identity provider (IdP); no single global endpoint is published.
  flow: authorizationCode
  name: oauth2AuthorizationCode
  sources:
  - https://developers.dexcarehealth.com/api/
  type: oauth2
- description: Publicly available information (clinic directories, provider listings, care-options discovery) is served without authentication.
  name: public
  sources:
  - https://developers.dexcarehealth.com/api/
  type: none
slug: dexcare-authentication
source_filename: dexcare-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developers.dexcarehealth.com/api/\ndocs: https://developers.dexcarehealth.com/api/\nsummary:\n  types: [oauth2, http, none]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  note: >-\n    Public endpoints returning non-sensitive directory information (clinics,\n    providers) require no authentication. Endpoints touching PHI/PII require a\n    JWT bearer token obtained via OAuth 2.0. Credentials and identity providers\n    are health-system specific; developers coordinate with each health system\n    for application credentials.\nschemes:\n  - name: bearerJWT\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    in: header\n    header: Authorization\n    description: >-\n      JSON Web Token passed as a bearer token in the Authorization header for\n      any endpoint that works with protected health information (PHI) or\n      personally identifiable information (PII).\n    sources: [https://developers.dexcarehealth.com/api/]\n\
  \  - name: oauth2AuthorizationCode\n    type: oauth2\n    flow: authorizationCode\n    description: >-\n      OAuth 2.0 Authorization Code Grant flow used to obtain the JWT bearer\n      token. Authorization and token endpoints are provided per health system\n      via that system's identity provider (IdP); no single global endpoint is\n      published.\n    sources: [https://developers.dexcarehealth.com/api/]\n  - name: public\n    type: none\n    description: >-\n      Publicly available information (clinic directories, provider listings,\n      care-options discovery) is served without authentication.\n    sources: [https://developers.dexcarehealth.com/api/]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dexcare/refs/heads/main/authentication/dexcare-authentication.yml
summary_line: oauth2/http/none · 3 schemes
tags:
- Company
- Healthcare
- Health IT
- Patient Access
- Scheduling
- Virtual Care
- Telehealth
- Care Navigation
- Provider Data
- SDK
---
