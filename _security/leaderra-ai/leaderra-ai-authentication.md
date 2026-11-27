---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Leaderra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Leaderra secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Leaderra
provider_slug: leaderra-ai
scheme_count: 1
schemes:
- description: 'API key as Bearer token — free key at https://leaderra.ai/signup (format: ldr_live_...)'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/leaderra-ai-openapi.yml
  type: http
slug: leaderra-ai-authentication
source_filename: leaderra-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: derived\nsource: openapi/leaderra-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key as Bearer token — free key at https://leaderra.ai/signup (format: ldr_live_...)'\n  sources:\n  - openapi/leaderra-ai-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/leaderra-ai/authentication/leaderra-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Sales
- Appointment-Setting
- Lead Generation
- B2B
---
