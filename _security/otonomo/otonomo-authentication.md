---
api_key_in: []
api_specs:
- filename: otonomo-fleet-openapi.yml
  format: yaml
  label: Otonomo Fleet API
  slug: otonomo-fleet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/otonomo/refs/heads/main/openapi/otonomo-fleet-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Otonomo Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Otonomo secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Otonomo
provider_slug: otonomo
scheme_count: 1
schemes:
- description: 'OAuth2 client-credentials. Obtain a Bearer token from POST /v1/oauth/token/ then send it as Authorization: Bearer <token>.'
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.otonomo.io/v1/oauth/token/
  name: oauth2
  sources:
  - openapi/otonomo-fleet-openapi.yml
  type: oauth2
slug: otonomo-authentication
source_filename: otonomo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/otonomo-fleet-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.otonomo.io/v1/oauth/token/\n    scopes: 0\n  description: 'OAuth2 client-credentials. Obtain a Bearer token from POST /v1/oauth/token/\n    then send it as Authorization: Bearer <token>.'\n  sources:\n  - openapi/otonomo-fleet-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/otonomo/refs/heads/main/authentication/otonomo-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Connected Vehicles
- Automotive
- Fleet Management
- Telematics
- Vehicle Data
- Mobility
- IoT
- Location
- Connected Car
---
