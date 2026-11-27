---
anonymous_access: false
api_key_in: []
api_specs:
- filename: muro-chat-ai-api-openapi.yml
  format: yaml
  label: muro AI API
  slug: muro-chat-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/muro-chat/openapi/muro-chat-ai-api-openapi.yml
- filename: muro-chat-automation-api-openapi.yml
  format: yaml
  label: muro Automation API
  slug: muro-chat-automation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/muro-chat/openapi/muro-chat-automation-api-openapi.yml
- filename: muro-chat-contacts-api-openapi.yml
  format: yaml
  label: muro Contacts API
  slug: muro-chat-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/muro-chat/openapi/muro-chat-contacts-api-openapi.yml
- filename: muro-chat-conversations-api-openapi.yml
  format: yaml
  label: muro Conversations API
  slug: muro-chat-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/muro-chat/openapi/muro-chat-conversations-api-openapi.yml
- filename: muro-chat-messages-api-openapi.yml
  format: yaml
  label: muro Messages API
  slug: muro-chat-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/muro-chat/openapi/muro-chat-messages-api-openapi.yml
- filename: muro-chat-meta-api-openapi.yml
  format: yaml
  label: muro Meta API
  slug: muro-chat-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/muro-chat/openapi/muro-chat-meta-api-openapi.yml
- filename: muro-chat-realtime-api-openapi.yml
  format: yaml
  label: muro Realtime API
  slug: muro-chat-realtime-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/muro-chat/openapi/muro-chat-realtime-api-openapi.yml
- filename: muro-chat-saved-replies-api-openapi.yml
  format: yaml
  label: muro Saved replies API
  slug: muro-chat-saved-replies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/muro-chat/openapi/muro-chat-saved-replies-api-openapi.yml
- filename: muro-chat-sites-api-openapi.yml
  format: yaml
  label: muro Sites API
  slug: muro-chat-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/muro-chat/openapi/muro-chat-sites-api-openapi.yml
- filename: muro-chat-webhooks-api-openapi.yml
  format: yaml
  label: muro Webhooks API
  slug: muro-chat-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/muro-chat/openapi/muro-chat-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: muro Authentication
name_suffix: Authentication
oauth_flows: []
overview: muro secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: muro
provider_slug: muro-chat
scheme_count: 1
schemes:
- description: 'A workspace API key, `Authorization: Bearer mr_live_…`. Scopes: read, write.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/muro-chat-openapi.json
  type: http
slug: muro-chat-authentication
source_filename: muro-chat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/muro-chat-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'A workspace API key, `Authorization: Bearer mr_live_…`. Scopes: read, write.'\n  sources:\n  - openapi/muro-chat-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/muro-chat/authentication/muro-chat-authentication.yml
summary_line: http · 1 scheme
tags:
- Live Chat
- Agency
- Resell
- Software-as-a-Service
---
