---
api_key_in: []
api_specs:
- filename: creatomate-openapi.yml
  format: yaml
  label: Creatomate Renders API
  slug: renders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatomate/refs/heads/main/openapi/creatomate-openapi.yml
- filename: creatomate-openapi.yml
  format: yaml
  label: Creatomate Templates API
  slug: templates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatomate/refs/heads/main/openapi/creatomate-openapi.yml
- filename: creatomate-openapi.yml
  format: yaml
  label: Creatomate Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatomate/refs/heads/main/openapi/creatomate-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Creatomate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Creatomate secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Creatomate
provider_slug: creatomate
scheme_count: 1
schemes:
- description: 'Project API key sent as `Authorization: Bearer <API_KEY>`. The key is found in the project settings of the Creatomate dashboard.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/creatomate-openapi.yml
  type: http
slug: creatomate-authentication
source_filename: creatomate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/creatomate-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Project API key sent as `Authorization: Bearer <API_KEY>`. The key is found\n    in the project settings of the Creatomate dashboard.'\n  sources:\n  - openapi/creatomate-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/creatomate/refs/heads/main/authentication/creatomate-authentication.yml
summary_line: http · 1 scheme
tags:
- Media
- Video Generation
- Image Generation
- Automation
- Templates
- Rendering
---
