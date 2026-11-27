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
name: BlogBat Authentication
name_suffix: Authentication
oauth_flows: []
overview: BlogBat secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BlogBat
provider_slug: blogbat-com
scheme_count: 1
schemes:
- description: API key obtained from POST /api/v1/agent/signup.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/blogbat-com-openapi.json
  type: http
slug: blogbat-com-authentication
source_filename: blogbat-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/blogbat-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key obtained from POST /api/v1/agent/signup.\n  sources:\n  - openapi/blogbat-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/blogbat-com/authentication/blogbat-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Blogging
- Artificial Intelligence
- SEO
- Multi-Tenant
- CustomDomain
---
