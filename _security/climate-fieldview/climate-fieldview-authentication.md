---
api_key_in: []
api_specs:
- filename: climate-fieldview-platform-openapi.yml
  format: yaml
  label: Climate FieldView Platform API
  slug: fieldview-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climate-fieldview/refs/heads/main/openapi/climate-fieldview-platform-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Climate Fieldview Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Climate FieldView secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Climate FieldView
provider_slug: climate-fieldview
scheme_count: 1
schemes:
- description: OAuth 2.0 authorization for Climate FieldView API
  flows:
  - authorizationUrl: https://api.climate.com/api/oauth/authorize
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://api.climate.com/api/oauth/token
  name: oauth2
  sources:
  - openapi/climate-fieldview-platform-openapi.yml
  type: oauth2
slug: climate-fieldview-authentication
source_filename: climate-fieldview-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/climate-fieldview-platform-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.climate.com/api/oauth/authorize\n    tokenUrl: https://api.climate.com/api/oauth/token\n    scopes: 5\n  description: OAuth 2.0 authorization for Climate FieldView API\n  sources:\n  - openapi/climate-fieldview-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/climate-fieldview/refs/heads/main/authentication/climate-fieldview-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Agriculture
- Bayer
- Crop Data
- Field Boundaries
- Harvest
- OAuth2
- Planting
- Precision Ag
---
