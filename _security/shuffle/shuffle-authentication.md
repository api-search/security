---
api_key_in: []
api_specs:
- filename: shuffle-openapi.yml
  format: yaml
  label: Shuffle API
  slug: shuffle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shuffle/refs/heads/main/openapi/shuffle-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Shuffle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shuffle secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Shuffle
provider_slug: shuffle
scheme_count: 1
schemes:
- description: 'API key obtained from Shuffle profile settings. Include as: Authorization: Bearer <APIKEY>'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/shuffle-openapi.yml
  type: http
slug: shuffle-authentication
source_filename: shuffle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shuffle-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key obtained from Shuffle profile settings. Include as: Authorization: Bearer\n    <APIKEY>'\n  sources:\n  - openapi/shuffle-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shuffle/refs/heads/main/authentication/shuffle-authentication.yml
summary_line: http · 1 scheme
tags:
- Security
- Workflows
- Automation
- SOAR
- Orchestration
- Open Source
---
