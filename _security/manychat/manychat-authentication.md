---
api_key_in: []
api_specs:
- filename: manychat-page-api-openapi.yml
  format: yaml
  label: ManyChat Page API
  slug: manychat-page-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/manychat/refs/heads/main/openapi/manychat-page-api-openapi.yml
- filename: manychat-sending-api-openapi.yml
  format: yaml
  label: ManyChat Sending API
  slug: manychat-sending-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/manychat/refs/heads/main/openapi/manychat-sending-api-openapi.yml
- filename: manychat-subscriber-api-openapi.yml
  format: yaml
  label: ManyChat Subscriber API
  slug: manychat-subscriber-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/manychat/refs/heads/main/openapi/manychat-subscriber-api-openapi.yml
- filename: manychat-template-api-openapi.yml
  format: yaml
  label: ManyChat Template API
  slug: manychat-template-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/manychat/refs/heads/main/openapi/manychat-template-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Manychat Authentication
name_suffix: Authentication
oauth_flows: []
overview: ManyChat secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ManyChat
provider_slug: manychat
scheme_count: 1
schemes:
- description: 'API key generated per page in the ManyChat dashboard under Settings > API. Sent as `Authorization: Bearer <page-id>:<api-key>`.'
  name: Bearer
  scheme: bearer
  sources:
  - openapi/manychat-page-api-openapi.yml
  - openapi/manychat-profile-api-openapi.yml
  - openapi/manychat-sending-api-openapi.yml
  - openapi/manychat-subscriber-api-openapi.yml
  type: http
slug: manychat-authentication
source_filename: manychat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/manychat-page-api-openapi.yml, openapi/manychat-profile-api-openapi.yml, openapi/manychat-sending-api-openapi.yml,\n  openapi/manychat-subscriber-api-openapi.yml\ndocs: https://help.manychat.com/hc/en-us/articles/14959510331420-API-Manychat\nnote: >-\n  ManyChat has exactly one credential type and no authorization surface at all. The token is an API key\n  generated per connected page in the ManyChat dashboard under Settings > API, sent as\n  `Authorization: Bearer <page-id>:<api-key>` — the page id is part of the credential, so the key is\n  intrinsically page-scoped and there is no account-wide or cross-page token. Verified against the\n  Swagger document ManyChat serves at https://api.manychat.com/swagger/compileJson?type=Page_API\n  on 2026-08-13; the linked help article is the provider's own reference but is currently unreadable to\n  non-browser clients (help.manychat.com returns 403 behind a Cloudflare challenge).\n\
  summary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  scopes: false\n  key_format: 'Bearer <page-id>:<api-key>'\n  key_scope: one connected page\n  rotation_documented: false\n  auth_failure_status_documented: false\nabsences:\n  - >-\n    No OAuth 2.0. There is no authorization endpoint, no token endpoint, no refresh, no scopes and no\n    consent screen — a third party cannot be delegated access on a user's behalf through the public API.\n    /.well-known/oauth-authorization-server returns 404 on api.manychat.com.\n  - No OpenID Connect. /.well-known/openid-configuration returns 404 on api.manychat.com.\n  - No mutual TLS, no request signing, no HMAC.\n  - >-\n    No 401 or 403 response is declared on ANY operation in the published spec despite every operation\n    requiring the Bearer token — the behaviour on a bad or revoked key is undocumented.\n  - No key rotation, expiry or revocation contract is published.\n\
  related_surface:\n  - >-\n    `verifyBySignedRequest` (POST /fb/subscriber/verifyBySignedRequest) verifies a Meta signed-request\n    payload to identify a subscriber. It authenticates the END USER inside a Messenger webview, not the\n    API caller, and still requires the page Bearer token itself.\n  - >-\n    The External Request / Dynamic Block callback surface has NO published authentication in either\n    direction — see asyncapi/manychat-dynamic-block-webhooks.yml.\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  description: 'API key generated per page in the ManyChat dashboard under Settings > API. Sent\n    as `Authorization: Bearer <page-id>:<api-key>`.'\n  sources:\n  - openapi/manychat-page-api-openapi.yml\n  - openapi/manychat-profile-api-openapi.yml\n  - openapi/manychat-sending-api-openapi.yml\n  - openapi/manychat-subscriber-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/manychat/refs/heads/main/authentication/manychat-authentication.yml
summary_line: http · 1 scheme
tags:
- Chat Marketing
- Messenger Marketing
- Conversational Commerce
- Marketing Automation
- Instagram
- WhatsApp
- Facebook Messenger
- SMS
- Chatbots
- Customer Engagement
- Automation
---
