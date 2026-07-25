---
api_key_in: []
api_specs:
- filename: flock-safety-alerts-api-openapi.yml
  format: yaml
  label: Flock Safety Alerts API
  slug: flock-safety-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/openapi/flock-safety-alerts-api-openapi.yml
- filename: flock-safety-cad-events-api-openapi.yml
  format: yaml
  label: Flock Safety CAD Events API
  slug: flock-safety-cad-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/openapi/flock-safety-cad-events-api-openapi.yml
- filename: flock-safety-custom-hotlists-api-openapi.yml
  format: yaml
  label: Flock Safety Custom Hotlists API
  slug: flock-safety-custom-hotlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/openapi/flock-safety-custom-hotlists-api-openapi.yml
- filename: flock-safety-devices-api-openapi.yml
  format: yaml
  label: Flock Safety Devices API
  slug: flock-safety-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/openapi/flock-safety-devices-api-openapi.yml
- filename: flock-safety-lpr-hotlist-alert-subscriptions-api-openapi.yml
  format: yaml
  label: Flock Safety LPR Hotlist Alert Subscriptions API
  slug: flock-safety-lpr-hotlist-alert-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/openapi/flock-safety-lpr-hotlist-alert-subscriptions-api-openapi.yml
- filename: flock-safety-oauth2-api-openapi.yml
  format: yaml
  label: Flock Safety OAuth2 API
  slug: flock-safety-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/openapi/flock-safety-oauth2-api-openapi.yml
- filename: flock-safety-plate-reads-api-openapi.yml
  format: yaml
  label: Flock Safety Plate Reads API
  slug: flock-safety-plate-reads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/openapi/flock-safety-plate-reads-api-openapi.yml
- filename: flock-safety-tracked-subject-types-api-openapi.yml
  format: yaml
  label: Flock Safety Tracked Subject Types API
  slug: flock-safety-tracked-subject-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/openapi/flock-safety-tracked-subject-types-api-openapi.yml
- filename: flock-safety-tracked-subjects-api-openapi.yml
  format: yaml
  label: Flock Safety Tracked Subjects API
  slug: flock-safety-tracked-subjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/openapi/flock-safety-tracked-subjects-api-openapi.yml
- filename: flock-safety-vehicle-images-api-openapi.yml
  format: yaml
  label: Flock Safety Vehicle Images API
  slug: flock-safety-vehicle-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/openapi/flock-safety-vehicle-images-api-openapi.yml
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
