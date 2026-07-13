---
api_key_in: []
api_specs:
- filename: source.yaml
  format: yaml
  label: Nifty Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://developers.niftypm.com/source.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nifty Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nifty secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nifty
provider_slug: nifty
scheme_count: 1
schemes:
- description: 'Bearer token authentication. Obtain an access token from the

    /token endpoint and pass it in the Authorization header as

    `Authorization: Bearer <token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/nifty-openapi.yml
  type: http
slug: nifty-authentication
source_filename: nifty-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nifty-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Bearer token authentication. Obtain an access token from the\n    /token endpoint and pass it in the Authorization header as\n    `Authorization: Bearer <token>`.\n  sources:\n  - openapi/nifty-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nifty/refs/heads/main/authentication/nifty-authentication.yml
summary_line: http · 1 scheme
tags:
- Project Management
- Task Management
- Collaboration
- Productivity
- Roadmaps
- Team Workspace
---
