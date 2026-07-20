---
api_key_in: []
api_specs:
- filename: ex-human-openapi.yml
  format: yaml
  label: Ex-Human API
  slug: ex-human-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ex-human/refs/heads/main/openapi/ex-human-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Ex Human Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ex-Human secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ex-Human
provider_slug: ex-human
scheme_count: 1
schemes:
- admin_url: https://admin.exh.ai/
  applied_to: all operations
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/ex-human-openapi.yml
  type: http
slug: ex-human-authentication
source_filename: ex-human-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/ex-human-openapi.yml\ndocs: https://docs.exh.ai/reference/getting-started-with-your-api\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  notes: >-\n    All Ex-Human API operations require an HTTP Bearer token. Create a Bearer token in the admin\n    console at https://admin.exh.ai/ and send it as `Authorization: Bearer <your-token>` on every\n    request. There is a single provider-wide security scheme (HTTPBearer); no OAuth 2.0, no OAuth\n    scopes, and no API-key query/header alternative are documented.\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  admin_url: https://admin.exh.ai/\n  applied_to: all operations\n  sources:\n  - openapi/ex-human-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ex-human/refs/heads/main/authentication/ex-human-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Conversational AI
- AI Companions
- Generative AI
- Text to Speech
- Image Generation
- Video Generation
- Avatars
- Multimodal
---
