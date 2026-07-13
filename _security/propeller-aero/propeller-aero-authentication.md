---
api_key_in: []
api_specs:
- filename: propeller-aero-openapi.yml
  format: yaml
  label: Propeller Organizations API
  slug: propeller-aero-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propeller-aero/refs/heads/main/openapi/propeller-aero-openapi.yml
- filename: propeller-aero-openapi.yml
  format: yaml
  label: Propeller Sites API
  slug: propeller-aero-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propeller-aero/refs/heads/main/openapi/propeller-aero-openapi.yml
- filename: propeller-aero-openapi.yml
  format: yaml
  label: Propeller Surveys API
  slug: propeller-aero-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propeller-aero/refs/heads/main/openapi/propeller-aero-openapi.yml
- filename: propeller-aero-openapi.yml
  format: yaml
  label: Propeller Workspaces API
  slug: propeller-aero-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propeller-aero/refs/heads/main/openapi/propeller-aero-openapi.yml
- filename: propeller-aero-openapi.yml
  format: yaml
  label: Propeller Shapes & Widgets API
  slug: propeller-aero-shapes-widgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propeller-aero/refs/heads/main/openapi/propeller-aero-openapi.yml
- filename: propeller-aero-openapi.yml
  format: yaml
  label: Propeller Position Monitoring API
  slug: propeller-aero-position-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propeller-aero/refs/heads/main/openapi/propeller-aero-openapi.yml
auth_types:
- http
- openIdConnect
description: ''
kind: authentication
layout: security
method: derived
name: Propeller Aero Authentication
name_suffix: Authentication
oauth_flows: []
overview: Propeller Aero secures its APIs with http and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Propeller Aero
provider_slug: propeller-aero
scheme_count: 2
schemes:
- description: 'Access token generated under Settings > Public API in the Propeller portal, sent as Authorization: Bearer <access_token>.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/propeller-aero-openapi.yml
  type: http
- name: oidc
  openIdConnectUrl: https://api.propelleraero.com/auth/oidc/.well-known/openid-configuration
  sources:
  - openapi/propeller-aero-openapi.yml
  type: openIdConnect
slug: propeller-aero-authentication
source_filename: propeller-aero-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/propeller-aero-openapi.yml\nsummary:\n  types:\n  - http\n  - openIdConnect\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Access token generated under Settings > Public API in the Propeller portal,\n    sent as Authorization: Bearer <access_token>.'\n  sources:\n  - openapi/propeller-aero-openapi.yml\n- name: oidc\n  type: openIdConnect\n  openIdConnectUrl: https://api.propelleraero.com/auth/oidc/.well-known/openid-configuration\n  sources:\n  - openapi/propeller-aero-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/propeller-aero/refs/heads/main/authentication/propeller-aero-authentication.yml
summary_line: http/openIdConnect · 2 schemes
tags:
- Drone Survey
- Geospatial
- Earthworks
- Construction
- Mining
- Photogrammetry
- Surveying
- Analytics
---
