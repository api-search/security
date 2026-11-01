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
name: Aicamp Authentication
name_suffix: Authentication
oauth_flows: []
overview: AICamp secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AICamp
provider_slug: aicamp
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/aicamp-openapi.json
  type: http
slug: aicamp-authentication
source_filename: aicamp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: derived\nsource: openapi/aicamp-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/aicamp-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/aicamp/authentication/aicamp-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Collaboration
- Workspace
- Team
- Platform
---
