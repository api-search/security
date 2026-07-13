---
api_key_in: []
api_specs:
- filename: sumo-logic-openapi.yml
  format: yaml
  label: Sumo Logic API
  slug: sumo-logic
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumo-logic/refs/heads/main/openapi/sumo-logic-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sumo Logic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sumo Logic secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sumo Logic
provider_slug: sumo-logic
scheme_count: 1
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/sumo-logic-openapi.yml
  type: http
slug: sumo-logic-authentication
source_filename: sumo-logic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sumo-logic-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/sumo-logic-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sumo-logic/refs/heads/main/authentication/sumo-logic-authentication.yml
summary_line: http · 1 scheme
tags:
- Logging
- Observability
- Security
- Monitoring
- Analytics
- DevOps
- SIEM
---
