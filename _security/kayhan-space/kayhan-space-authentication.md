---
api_key_in: []
api_specs:
- filename: kayhan-space-satcat-openapi-original.json
  format: json
  label: Satcat Service API
  slug: satcat-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kayhan-space/refs/heads/main/openapi/kayhan-space-satcat-openapi-original.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Kayhan Space Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- password
overview: Kayhan Space secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and password flow(s).
provider_name: Kayhan Space
provider_slug: kayhan-space
scheme_count: 1
schemes:
- flows:
  - flow: password
    scopes: 1
    tokenUrl: login
  - flow: clientCredentials
    scopes: 1
    tokenUrl: oauth/token
  name: Oauth2Scheme
  sources:
  - openapi/kayhan-space-satcat-openapi-original.json
  type: oauth2
slug: kayhan-space-authentication
source_filename: kayhan-space-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/kayhan-space-satcat-openapi-original.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  - password\nschemes:\n- name: Oauth2Scheme\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: login\n    scopes: 1\n  - flow: clientCredentials\n    tokenUrl: oauth/token\n    scopes: 1\n  sources:\n  - openapi/kayhan-space-satcat-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kayhan-space/refs/heads/main/authentication/kayhan-space-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Frontier Tech
- Space
- Satellite
- Space Situational Awareness
- Collision Avoidance
- Space Traffic Management
- Aerospace
- Astrodynamics
---
