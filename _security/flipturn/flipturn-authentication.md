---
api_key_in: []
api_specs:
- filename: flipturn-openapi.yml
  format: yaml
  label: Flipturn API
  slug: flipturn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipturn/refs/heads/main/openapi/flipturn-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Flipturn Authentication
name_suffix: Authentication
oauth_flows: []
overview: Flipturn secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Flipturn
provider_slug: flipturn
scheme_count: 1
schemes:
- description: 'API key passed as a bearer token in the Authorization header: `Authorization: Bearer {api_key}`. Keys are created in the Flipturn app (Manage > API Keys) by an Owner and can be scoped to specific sites or chargers.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/flipturn-openapi.yml
  type: http
slug: flipturn-authentication
source_filename: flipturn-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/flipturn-openapi.yml\ndocs: https://api-docs.getflipturn.com/authorization.md\nnotes: >-\n  Flipturn uses a single bearer API key passed in the Authorization header\n  (`Authorization: Bearer {api_key}`). API keys are created in the Flipturn app\n  (cloud.getflipturn.com > Manage > API Keys) by an Owner-level user and can be\n  scoped to a specific site or subset of chargers. There is no OAuth or OpenID\n  Connect surface.\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key passed as a bearer token in the Authorization header: `Authorization:\n    Bearer {api_key}`. Keys are created in the Flipturn app (Manage > API Keys) by an Owner\n    and can be scoped to specific sites or chargers.'\n  sources:\n  - openapi/flipturn-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flipturn/refs/heads/main/authentication/flipturn-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- EV Charging
- Electric Vehicles
- Fleet Management
- Energy
- Charging Infrastructure
- OCPP
- OCPI
- Mobility
- REST API
---
