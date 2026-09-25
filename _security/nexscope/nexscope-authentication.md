---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nexscope-openapi.json
  format: json
  label: Nexscope Ecommerce Data and Creative APIs
  slug: nexscope-ecommerce-data-and-creative-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexscope/refs/heads/main/openapi/nexscope-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Nexscope Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nexscope Ecommerce Data and Creative APIs secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nexscope Ecommerce Data and Creative APIs
provider_slug: nexscope
scheme_count: 1
schemes:
- bearerFormat: Nexscope API Key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/nexscope-openapi.json
  type: http
slug: nexscope-authentication
source_filename: nexscope-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: derived\nsource: openapi/nexscope-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Nexscope API Key\n  sources:\n  - openapi/nexscope-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexscope/refs/heads/main/authentication/nexscope-authentication.yml
summary_line: http · 1 scheme
tags:
- E-Commerce
- Data
- Creative
- Artificial Intelligence
- Marketplace Intelligence
- Amazon
- TikTok
- Keyword Research
- Image Generation
- Video Generation
- MCP
---
