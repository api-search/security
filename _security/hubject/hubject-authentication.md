---
anonymous_access: false
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Hubject Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Hubject secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Hubject
provider_slug: hubject
scheme_count: 1
schemes:
- description: OAuth2 is used to grant access to the endpoint.
  flows:
  - flow: authorizationCode
    scopes: 0
  name: MO
  sources:
  - openapi/hubject-opcp-ccp-openapi.json
  - openapi/hubject-opcp-cps-openapi.json
  - openapi/hubject-opcp-est-openapi.json
  - openapi/hubject-opcp-pcp-openapi.json
  - openapi/hubject-opcp-rcp-openapi.json
  type: oauth2
slug: hubject-authentication
source_filename: hubject-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: derived\nsource: openapi/hubject-opcp-ccp-openapi.json, openapi/hubject-opcp-cps-openapi.json, openapi/hubject-opcp-est-openapi.json,\n  openapi/hubject-opcp-pcp-openapi.json, openapi/hubject-opcp-rcp-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: MO\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    scopes: 0\n  description: OAuth2 is used to grant access to the endpoint.\n  sources:\n  - openapi/hubject-opcp-ccp-openapi.json\n  - openapi/hubject-opcp-cps-openapi.json\n  - openapi/hubject-opcp-est-openapi.json\n  - openapi/hubject-opcp-pcp-openapi.json\n  - openapi/hubject-opcp-rcp-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/hubject/authentication/hubject-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- E-Mobility
- EV Charging
- Interoperability
---
