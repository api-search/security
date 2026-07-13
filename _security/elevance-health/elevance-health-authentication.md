---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Elevance Health Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Elevance Health secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Elevance Health
provider_slug: elevance-health
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://patient360c.anthem.com/P360Member/oauth2/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://patient360c.anthem.com/P360Member/oauth2/token
  name: oauth2
  sources:
  - openapi/elevance-health-openapi.yml
  type: oauth2
slug: elevance-health-authentication
source_filename: elevance-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/elevance-health-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://patient360c.anthem.com/P360Member/oauth2/authorize\n    tokenUrl: https://patient360c.anthem.com/P360Member/oauth2/token\n    scopes: 3\n  sources:\n  - openapi/elevance-health-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elevance-health/refs/heads/main/authentication/elevance-health-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Fortune 500
- Healthcare
- Health Insurance
- FHIR
- Interoperability
---
