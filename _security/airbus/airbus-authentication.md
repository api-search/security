---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Airbus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Airbus secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Airbus
provider_slug: airbus
scheme_count: 1
schemes:
- description: 'Bearer access token obtained via POST

    /auth/realms/IDP/protocol/openid-connect/token with grant_type=api_key.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/airbus-openapi.yml
  type: http
slug: airbus-authentication
source_filename: airbus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/airbus-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Bearer access token obtained via POST\n    /auth/realms/IDP/protocol/openid-connect/token with grant_type=api_key.\n  sources:\n  - openapi/airbus-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airbus/refs/heads/main/authentication/airbus-authentication.yml
summary_line: http · 1 scheme
tags:
- Aerospace
- Defense
- Manufacturing
- Aviation
- Earth Observation
- Satellite Imagery
---
