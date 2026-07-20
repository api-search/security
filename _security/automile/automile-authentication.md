---
api_key_in: []
api_specs:
- filename: automile-openapi-original.json
  format: json
  label: Automile API
  slug: automile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automile/refs/heads/main/openapi/automile-openapi-original.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Automile Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Automile secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Automile
provider_slug: automile
scheme_count: 1
schemes:
- description: OAuth2 Implicit Grant
  flows:
  - authorizationUrl: https://api.automile.com/login/
    flow: implicit
    scopes: 2
  name: oauth2
  sources:
  - openapi/automile-openapi-original.json
  type: oauth2
slug: automile-authentication
source_filename: automile-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/automile-openapi-original.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://api.automile.com/login/\n    scopes: 2\n  description: OAuth2 Implicit Grant\n  sources:\n  - openapi/automile-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/automile/refs/heads/main/authentication/automile-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Fleet Management
- Telematics
- GPS Tracking
- Vehicles
- Transportation
- Mileage
- IoT
- Logistics
- Company
---
