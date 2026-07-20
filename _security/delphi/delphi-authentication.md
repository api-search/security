---
api_key_in:
- header
api_specs:
- filename: delphi-openapi.yml
  format: yaml
  label: Delphi API
  slug: delphi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delphi/refs/heads/main/openapi/delphi-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Delphi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Delphi secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Delphi
provider_slug: delphi
scheme_count: 1
schemes:
- clone_scoped: true
  description: API key scoped to a single clone. Available on the Immortal plan; request one from support@delphi.ai.
  docs: https://docs.delphi.ai/advanced/actions/api-immortal-only
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  provisioning: Immortal plan; request from support@delphi.ai (shown once)
  sources:
  - openapi/delphi-openapi.yml
  type: apiKey
slug: delphi-authentication
source_filename: delphi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/delphi-openapi.yml\ndocs: https://docs.delphi.ai/advanced/actions/api-immortal-only\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nnotes: >-\n  Delphi uses a single API-key scheme (no OAuth, no scopes). Every request\n  carries an x-api-key header. The key is scoped to a single clone — it can\n  only interact with conversations and users belonging to that clone. API\n  access is available on the Immortal plan; keys are provisioned by Delphi\n  (email support@delphi.ai) and shown only once. Webhook deliveries are\n  authenticated separately with an HMAC signing secret (see asyncapi/).\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  clone_scoped: true\n  provisioning: Immortal plan; request from support@delphi.ai (shown once)\n  docs: https://docs.delphi.ai/advanced/actions/api-immortal-only\n  description: API key scoped to a single clone. Available on the Immortal\
  \ plan; request one\n    from support@delphi.ai.\n  sources:\n  - openapi/delphi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/delphi/refs/heads/main/authentication/delphi-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- AI Clones
- Digital Minds
- Conversational AI
- Voice
- Search
- RAG
- Knowledge Base
- Creator Economy
- Webhooks
---
