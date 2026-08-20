---
api_key_in:
- header
api_specs:
- filename: fixie-accounts-api-openapi.yml
  format: yaml
  label: Fixie accounts API
  slug: fixie-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixie/refs/heads/main/openapi/fixie-accounts-api-openapi.yml
- filename: fixie-agents-api-openapi.yml
  format: yaml
  label: Fixie agents API
  slug: fixie-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixie/refs/heads/main/openapi/fixie-agents-api-openapi.yml
- filename: fixie-api-keys-api-openapi.yml
  format: yaml
  label: Fixie api_keys API
  slug: fixie-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixie/refs/heads/main/openapi/fixie-api-keys-api-openapi.yml
- filename: fixie-call-throttles-api-openapi.yml
  format: yaml
  label: Fixie call_throttles API
  slug: fixie-call-throttles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixie/refs/heads/main/openapi/fixie-call-throttles-api-openapi.yml
- filename: fixie-calls-api-openapi.yml
  format: yaml
  label: Fixie calls API
  slug: fixie-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixie/refs/heads/main/openapi/fixie-calls-api-openapi.yml
- filename: fixie-corpora-api-openapi.yml
  format: yaml
  label: Fixie corpora API
  slug: fixie-corpora-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixie/refs/heads/main/openapi/fixie-corpora-api-openapi.yml
- filename: fixie-deleted-calls-api-openapi.yml
  format: yaml
  label: Fixie deleted_calls API
  slug: fixie-deleted-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixie/refs/heads/main/openapi/fixie-deleted-calls-api-openapi.yml
- filename: fixie-models-api-openapi.yml
  format: yaml
  label: Fixie models API
  slug: fixie-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixie/refs/heads/main/openapi/fixie-models-api-openapi.yml
- filename: fixie-schema-api-openapi.yml
  format: yaml
  label: Fixie schema API
  slug: fixie-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixie/refs/heads/main/openapi/fixie-schema-api-openapi.yml
- filename: fixie-sip-api-openapi.yml
  format: yaml
  label: Fixie sip API
  slug: fixie-sip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixie/refs/heads/main/openapi/fixie-sip-api-openapi.yml
- filename: fixie-telephony-configs-api-openapi.yml
  format: yaml
  label: Fixie telephony_configs API
  slug: fixie-telephony-configs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixie/refs/heads/main/openapi/fixie-telephony-configs-api-openapi.yml
- filename: fixie-tools-api-openapi.yml
  format: yaml
  label: Fixie tools API
  slug: fixie-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixie/refs/heads/main/openapi/fixie-tools-api-openapi.yml
- filename: fixie-voices-api-openapi.yml
  format: yaml
  label: Fixie voices API
  slug: fixie-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixie/refs/heads/main/openapi/fixie-voices-api-openapi.yml
- filename: fixie-webhooks-api-openapi.yml
  format: yaml
  label: Fixie webhooks API
  slug: fixie-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixie/refs/heads/main/openapi/fixie-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Fixie Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fixie secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fixie
provider_slug: fixie
scheme_count: 1
schemes:
- description: API key
  in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/fixie-ultravox-openapi-original.yml
  type: apiKey
slug: fixie-authentication
source_filename: fixie-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/fixie-ultravox-openapi-original.yml\ndocs: https://docs.ultravox.ai/gettingstarted/quickstart/api-key\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  notes: >-\n    Single auth model — a 41-character API key (8 chars + '.' + 32 chars) sent\n    in the X-API-Key request header. No OAuth or OIDC; there is no scope surface.\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key\n  sources:\n  - openapi/fixie-ultravox-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fixie/refs/heads/main/authentication/fixie-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Voice AI
- Conversational AI
- Real-Time
- Speech
- Agents
- Telephony
- Machine-Learning
- SIP
- Webhook
---
