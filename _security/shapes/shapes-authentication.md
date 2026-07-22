---
api_key_in: []
api_specs:
- filename: shapes-api-openapi.yml
  format: yaml
  label: Shapes API
  slug: shapes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapes/refs/heads/main/openapi/shapes-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Shapes Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shapes secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Shapes
provider_slug: shapes
scheme_count: 1
schemes:
- description: 'API key generated at https://shapes.inc/developer, sent as the HTTP header `Authorization: Bearer <API-key>`. Also read from the SHAPESINC_API_KEY environment variable in the official examples. By default the API treats the caller as the key owner.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/shapes-api-openapi.yml
  type: http
slug: shapes-authentication
source_filename: shapes-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/shapes-api-openapi.yml\ndocs: https://github.com/shapesinc/shapes-api\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    API key generated at https://shapes.inc/developer, sent as the HTTP header\n    `Authorization: Bearer <API-key>`. Also read from the SHAPESINC_API_KEY environment variable in the\n    official examples. By default the API treats the caller as the key owner.\n  sources:\n  - openapi/shapes-api-openapi.yml\ncustom_headers:\n- name: X-User-Id\n  purpose: End-user identification; isolates conversation context and Shape memory per user. Strongly recommended for user-facing apps.\n- name: X-Channel-Id\n  purpose: Conversation/channel context for apps that support more than one conversation per user.\nnotes:\n  - The public GET /shapes/public/{username} endpoint requires no authentication.\n  - >-\n    Shapes also supports an OAuth-style \"\
  Shapes authorization\" that links API conversations to a user's\n    shapes.inc account (memory + personas), documented via the shape-auth-example in the repo.\n  - The Shapes developer API was deprecated 2025-09-25; keys may no longer be issued.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shapes/refs/heads/main/authentication/shapes-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- AI Agents
- Chat
- Social
- Conversational AI
- LLM
- Voice
- Developer API
---
