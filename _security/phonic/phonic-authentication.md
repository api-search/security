---
api_key_in: []
api_specs:
- filename: phonic-agents-api-openapi.yml
  format: yaml
  label: Phonic agents API
  slug: phonic-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phonic/refs/heads/main/openapi/phonic-agents-api-openapi.yml
- filename: phonic-apikeys-api-openapi.yml
  format: yaml
  label: Phonic apiKeys API
  slug: phonic-apikeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phonic/refs/heads/main/openapi/phonic-apikeys-api-openapi.yml
- filename: phonic-auth-api-openapi.yml
  format: yaml
  label: Phonic auth API
  slug: phonic-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phonic/refs/heads/main/openapi/phonic-auth-api-openapi.yml
- filename: phonic-conversationitems-api-openapi.yml
  format: yaml
  label: Phonic conversationItems API
  slug: phonic-conversationitems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phonic/refs/heads/main/openapi/phonic-conversationitems-api-openapi.yml
- filename: phonic-conversations-api-openapi.yml
  format: yaml
  label: Phonic conversations API
  slug: phonic-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phonic/refs/heads/main/openapi/phonic-conversations-api-openapi.yml
- filename: phonic-extractionschemas-api-openapi.yml
  format: yaml
  label: Phonic extractionSchemas API
  slug: phonic-extractionschemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phonic/refs/heads/main/openapi/phonic-extractionschemas-api-openapi.yml
- filename: phonic-projects-api-openapi.yml
  format: yaml
  label: Phonic projects API
  slug: phonic-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phonic/refs/heads/main/openapi/phonic-projects-api-openapi.yml
- filename: phonic-tools-api-openapi.yml
  format: yaml
  label: Phonic tools API
  slug: phonic-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phonic/refs/heads/main/openapi/phonic-tools-api-openapi.yml
- filename: phonic-voices-api-openapi.yml
  format: yaml
  label: Phonic voices API
  slug: phonic-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phonic/refs/heads/main/openapi/phonic-voices-api-openapi.yml
- filename: phonic-workspace-api-openapi.yml
  format: yaml
  label: Phonic workspace API
  slug: phonic-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phonic/refs/heads/main/openapi/phonic-workspace-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Phonic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Phonic secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Phonic
provider_slug: phonic
scheme_count: 1
schemes:
- description: Bearer authentication header of the form `Bearer <PHONIC_API_KEY>`. Manage your API keys at https://phonic.co/api-keys.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/phonic-openapi-original.yaml
  type: http
slug: phonic-authentication
source_filename: phonic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/phonic-openapi-original.yaml\ndocs: https://docs.phonic.co/docs/authentication/overview\nsummary:\n  types:\n  - http\n  mechanisms:\n  - api-key\n  - session-token\n  - jwt\n  transport:\n    rest: 'Authorization: Bearer <PHONIC_API_KEY or JWT>'\n    websocket: 'wss://api.phonic.ai/v1/sts/ws?session_token=<token> (or ?jwt=<jwt>)'\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer authentication header of the form `Bearer <PHONIC_API_KEY>`. Manage your\n    API keys at https://phonic.co/api-keys.\n  sources:\n  - openapi/phonic-openapi-original.yaml\nmechanisms:\n- id: api-key\n  lifetime: permanent\n  minted_by: You, in the Phonic dashboard\n  use_when: Server-to-server calls. Never expose to a browser.\n  passed_as: 'Authorization: Bearer <PHONIC_API_KEY>'\n  manage_url: https://phonic.co/api-keys\n- id: session-token\n  lifetime: 60s to 1h\n  minted_by: Phonic, minted from your API\
  \ key\n  use_when: Browser or mobile clients where you do not want to ship your API key. Simple to revoke.\n  minted_via: openapi/phonic-openapi-original.yaml#POST /auth/session_token\n  docs: https://docs.phonic.co/docs/authentication/session-tokens\n- id: jwt\n  lifetime: You choose (recommended <= 15 min)\n  minted_by: Your own auth system (signed with your key; Phonic verifies without a round-trip)\n  use_when: Enterprise integrations with an existing identity system needing per-user / per-conversation scoping.\n  minted_via: openapi/phonic-openapi-original.yaml#POST /auth/conversation_token\n  docs: https://docs.phonic.co/docs/authentication/jw-ts\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phonic/refs/heads/main/authentication/phonic-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Voice AI
- Conversational AI
- Speech
- Voice Agents
- Telephony
- Speech to Speech
---
