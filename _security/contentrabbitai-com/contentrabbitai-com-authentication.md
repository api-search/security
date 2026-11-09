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
name: Contentrabbitai Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Content Rabbit secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Content Rabbit
provider_slug: contentrabbitai-com
scheme_count: 1
schemes:
- description: API key obtained from POST /api/v1/agent/signup.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/contentrabbitai-com-openapi.json
  type: http
slug: contentrabbitai-com-authentication
source_filename: contentrabbitai-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/contentrabbitai-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key obtained from POST /api/v1/agent/signup.\n  sources:\n  - openapi/contentrabbitai-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/contentrabbitai-com/authentication/contentrabbitai-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Software-as-a-Service
- Social Media
- Artificial Intelligence
- Content Management
- Automation
---
