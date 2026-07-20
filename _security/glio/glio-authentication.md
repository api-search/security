---
api_key_in: []
api_specs:
- filename: glio-openapi-original.json
  format: json
  label: Glio API
  slug: glio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glio/refs/heads/main/openapi/glio-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Glio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Glio secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Glio
provider_slug: glio
scheme_count: 1
schemes:
- bearerFormat: API Key or JWT
  description: 'API key or JWT token: `Bearer <your-token>`'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/glio-openapi-original.json
  type: http
slug: glio-authentication
source_filename: glio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/glio-openapi-original.json\ndocs: https://glio.io/docs/getting-started\nnotes: >-\n  Single scheme. All endpoints require an Authorization: Bearer header carrying\n  either a Glio API key or a JWT. No OAuth 2.0 / OpenID Connect scope surface is\n  published; API keys are issued from the dashboard at https://glio.io/app/.\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key or JWT\n  description: 'API key or JWT token: `Bearer <your-token>`'\n  sources:\n  - openapi/glio-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glio/refs/heads/main/authentication/glio-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI
- Machine Learning
- Media Generation
- Video Generation
- Image Generation
- Audio Generation
- Text to Speech
- Large Language Models
- Generative AI
- API Aggregator
- Developer Tools
---
