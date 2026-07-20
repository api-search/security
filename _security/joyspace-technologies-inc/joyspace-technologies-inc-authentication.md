---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Joyspace Technologies Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: JoySpace Technologies, Inc. secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: JoySpace Technologies, Inc.
provider_slug: joyspace-technologies-inc
scheme_count: 1
schemes:
- format: 'Authorization: Bearer [example key]'
  header: Authorization
  in: header
  name: bearerApiKey
  scheme: bearer
  sources:
  - https://joyspace.ai/enterprise/api
  type: http
slug: joyspace-technologies-inc-authentication
source_filename: joyspace-technologies-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://joyspace.ai/enterprise/api\ndocs: https://joyspace.ai/enterprise/api\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  notes: >-\n    The Joyspace REST API authenticates with a Bearer API key passed in the\n    Authorization header. No OpenAPI/Swagger document is published, so this\n    profile is captured verbatim from the developer documentation rather than\n    derived from a spec.\nschemes:\n  - name: bearerApiKey\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: 'Authorization: Bearer [example key]'\n    sources: [https://joyspace.ai/enterprise/api]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/joyspace-technologies-inc/refs/heads/main/authentication/joyspace-technologies-inc-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Video
- Artificial Intelligence
- Video Processing
- Content Creation
- Media
- Webhooks
- Enterprise
---
