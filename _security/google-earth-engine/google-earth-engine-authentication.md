---
api_key_in: []
api_specs:
- filename: earth-engine.yml
  format: yaml
  label: Google Earth Engine REST API v1
  slug: google-earth-engine-rest-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-earth-engine/refs/heads/main/openapi/earth-engine.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Earth Engine Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Earth Engine REST secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Earth Engine REST
provider_slug: google-earth-engine
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/earth-engine.yml
  type: oauth2
slug: google-earth-engine-authentication
source_filename: google-earth-engine-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/earth-engine.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 3\n  sources:\n  - openapi/earth-engine.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-earth-engine/refs/heads/main/authentication/google-earth-engine-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Climate
- Earth Observation
- Environmental
- Geospatial
- GIS
- Google
- Remote Sensing
- Satellite Imagery
---
