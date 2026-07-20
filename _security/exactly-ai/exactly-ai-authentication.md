---
api_key_in: []
api_specs:
- filename: exactly-ai-public-openapi-original.json
  format: json
  label: Exactly Public API
  slug: exactly-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exactly-ai/refs/heads/main/openapi/exactly-ai-public-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Exactly Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Exactly Ai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Exactly Ai
provider_slug: exactly-ai
scheme_count: 1
schemes:
- name: APITokenAuth
  scheme: bearer
  sources:
  - openapi/exactly-ai-public-openapi-original.json
  type: http
slug: exactly-ai-authentication
source_filename: exactly-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/exactly-ai-public-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: APITokenAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/exactly-ai-public-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exactly-ai/refs/heads/main/authentication/exactly-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Image Generation
- Generative AI
- Creative Tools
- Brand
- Machine Learning
- Media
---
