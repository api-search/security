---
api_key_in: []
api_specs:
- filename: flock-safety-openapi-original.yml
  format: yaml
  label: Flock Safety API Platform (v3)
  slug: flock-safety-api-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/openapi/flock-safety-openapi-original.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Flock Safety Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Flock Safety secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Flock Safety
provider_slug: flock-safety
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/flock-safety-openapi-original.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://api.flocksafety.com/oauth/token
  name: oauth2Auth
  sources:
  - openapi/flock-safety-openapi-original.yml
  type: oauth2
slug: flock-safety-authentication
source_filename: flock-safety-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/flock-safety-openapi-original.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/flock-safety-openapi-original.yml\n- name: oauth2Auth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.flocksafety.com/oauth/token\n    scopes: 2\n  sources:\n  - openapi/flock-safety-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/authentication/flock-safety-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- American Dynamism
- Public Safety
- Law Enforcement
- License Plate Recognition
- LPR
- Physical Security
- Surveillance
- Computer Vision
- Webhooks
- Geolocation
- CAD
---
