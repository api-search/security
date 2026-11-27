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
name: Kubflow AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kubflow AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kubflow AI
provider_slug: kubflow-ai
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/kubflow-ai-openapi.json
  type: http
slug: kubflow-ai-authentication
source_filename: kubflow-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: derived\nsource: openapi/kubflow-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/kubflow-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/kubflow-ai/authentication/kubflow-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Media Generation
- Marketing
- Automation
- Platform
- Image
- Video
---
