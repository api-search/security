---
api_key_in:
- header
api_specs:
- filename: zavu-openapi-original.json
  format: json
  label: Zavu Unified Messaging Layer API
  slug: zavu-unified-messaging-layer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zavu/refs/heads/main/openapi/zavu-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Zavu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zavu secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zavu
provider_slug: zavu
scheme_count: 1
schemes:
- bearerFormat: JWT
  env: ZAVUDEV_API_KEY
  format: Bearer <api_key>
  header: Authorization
  key_prefixes:
    live: zv_live_
    test: zv_test_
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/zavu-openapi-original.json
  type: http
slug: zavu-authentication
source_filename: zavu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource:\n  - https://docs.zavu.dev/authentication.md\n  - openapi/zavu-openapi-original.json\ndocs: https://docs.zavu.dev/authentication.md\nsummary:\n  types:\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  header: Authorization\n  format: \"Bearer <api_key>\"\n  key_prefixes:\n    live: zv_live_\n    test: zv_test_\n  env: ZAVUDEV_API_KEY\n  sources:\n  - openapi/zavu-openapi-original.json\nnotes: >-\n  Zavu uses opaque API-key bearer tokens (prefixed zv_live_ / zv_test_) rather\n  than a full OAuth2 flow, so there is no OAuth scope surface (scopes/ skipped).\n  Keys are project/team-scoped; the account context endpoint (getCurrentApiKeyContext)\n  resolves the project bound to a key.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zavu/refs/heads/main/authentication/zavu-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Messaging
- SMS
- WhatsApp
- Email
- Voice
- Communications
- CPaaS
- Webhooks
- AI Agents
---
