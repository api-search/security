---
api_key_in: []
api_specs:
- filename: notdiamond-openapi.yml
  format: yaml
  label: Not Diamond Model Select API
  slug: notdiamond-model-select-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notdiamond/refs/heads/main/openapi/notdiamond-openapi.yml
- filename: notdiamond-openapi.yml
  format: yaml
  label: Not Diamond Models API
  slug: notdiamond-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notdiamond/refs/heads/main/openapi/notdiamond-openapi.yml
- filename: notdiamond-openapi.yml
  format: yaml
  label: Not Diamond Feedback API
  slug: notdiamond-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notdiamond/refs/heads/main/openapi/notdiamond-openapi.yml
- filename: notdiamond-openapi.yml
  format: yaml
  label: Not Diamond Custom Routers API
  slug: notdiamond-custom-routers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notdiamond/refs/heads/main/openapi/notdiamond-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Notdiamond Authentication
name_suffix: Authentication
oauth_flows: []
overview: Not Diamond secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Not Diamond
provider_slug: notdiamond
scheme_count: 1
schemes:
- description: Not Diamond API key passed as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/notdiamond-openapi.yml
  type: http
slug: notdiamond-authentication
source_filename: notdiamond-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/notdiamond-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Not Diamond API key passed as a Bearer token.\n  sources:\n  - openapi/notdiamond-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/notdiamond/refs/heads/main/authentication/notdiamond-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- Model Routing
- Router
- Orchestration
---
