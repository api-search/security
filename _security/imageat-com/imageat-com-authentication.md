---
anonymous_access: false
api_key_in: []
api_specs:
- filename: imageat-com-images-api-openapi.yml
  format: yaml
  label: imageat Images API
  slug: imageat-com-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imageat-com/openapi/imageat-com-images-api-openapi.yml
- filename: imageat-com-models-api-openapi.yml
  format: yaml
  label: imageat Models API
  slug: imageat-com-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imageat-com/openapi/imageat-com-models-api-openapi.yml
- filename: imageat-com-responses-api-openapi.yml
  format: yaml
  label: imageat Responses API
  slug: imageat-com-responses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imageat-com/openapi/imageat-com-responses-api-openapi.yml
- filename: imageat-com-social-api-openapi.yml
  format: yaml
  label: imageat Social API
  slug: imageat-com-social-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imageat-com/openapi/imageat-com-social-api-openapi.yml
- filename: imageat-com-videos-api-openapi.yml
  format: yaml
  label: imageat Videos API
  slug: imageat-com-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imageat-com/openapi/imageat-com-videos-api-openapi.yml
- filename: imageat-com-chat-completions-api-openapi.yml
  format: yaml
  label: imageat Chat Completions API
  slug: imageat-com-chat-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imageat-com/openapi/imageat-com-chat-completions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: imageat Authentication
name_suffix: Authentication
oauth_flows: []
overview: imageat secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: imageat
provider_slug: imageat-com
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/imageat-com-openapi.yml
  type: http
slug: imageat-com-authentication
source_filename: imageat-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/imageat-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/imageat-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/imageat-com/authentication/imageat-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Image Generation
- Video Generation
- Agentic Workflows
- No-Code
---
