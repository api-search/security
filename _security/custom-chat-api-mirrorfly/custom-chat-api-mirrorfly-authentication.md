---
anonymous_access: false
api_key_in: []
auth_types:
- custom-token
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Custom Chat Api Mirrorfly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Custom Chat API | MirrorFly secures its APIs with custom-token across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Custom Chat API | MirrorFly
provider_slug: custom-chat-api-mirrorfly
scheme_count: 1
schemes:
- description: Short-lived (1 hour) token returned by POST /api/v1/login using console-issued username and password; sent on secured endpoints via the Authorization header. Expired tokens return 401.
  name: PlatformApiToken
  scheme: bearer-like custom token
  sources:
  - https://www.mirrorfly.com/docs/platformapi/userapis/getstarted/login/
  - https://www.mirrorfly.com/docs/platformapi/adminapis/get-started/
  type: http
slug: custom-chat-api-mirrorfly-authentication
source_filename: custom-chat-api-mirrorfly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\nsource: https://www.mirrorfly.com/docs/platformapi/adminapis/get-started/\ndocs: https://www.mirrorfly.com/docs/platformapi/userapis/getstarted/login/\nnote: >-\n  No OpenAPI exists to derive from; this profile is read from the provider's Platform API docs.\n  Authentication is a custom short-lived bearer token, not OAuth: POST /api/v1/login with the\n  static username/password issued in the MirrorFly console (shown after server configuration for\n  Eazy-plan and paid subscribers) returns a token valid for up to 1 hour. Secured endpoints send\n  that token in the Authorization header; on a 401 the client must call login again for a fresh\n  token. There are separate User API and Admin API credentials, both following the same flow.\nsummary:\n  types: [custom-token]\n  token_endpoint: POST /api/v1/login\n  token_ttl_seconds: 3600\n  header: Authorization\n  oauth2_flows: []\nschemes:\n- name: PlatformApiToken\n  type: http\n  scheme:\
  \ bearer-like custom token\n  description: >-\n    Short-lived (1 hour) token returned by POST /api/v1/login using console-issued username and\n    password; sent on secured endpoints via the Authorization header. Expired tokens return 401.\n  sources:\n  - https://www.mirrorfly.com/docs/platformapi/userapis/getstarted/login/\n  - https://www.mirrorfly.com/docs/platformapi/adminapis/get-started/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/custom-chat-api-mirrorfly/refs/heads/main/authentication/custom-chat-api-mirrorfly-authentication.yml
summary_line: custom-token · 1 scheme
tags:
- Chat API
- Messaging
- CPaaS
- VoIP
- Voice
- Video Calling
- Contact Center
- Conversational AI
- Chatbots
- Live Streaming
---
