---
api_key_in: []
api_specs:
- filename: Public-APIs
  format: yaml
  label: Kore.ai AI for Service Platform APIs
  slug: koreai-ai-for-service-platform-apis
  spec_type: Postman
  url: https://github.com/Koredotcom/Public-APIs
- filename: koreai-chat-api-openapi.yml
  format: yaml
  label: Kore.ai Chat API
  slug: koreai-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koreai/refs/heads/main/openapi/koreai-chat-api-openapi.yml
- filename: koreai-conversation-api-openapi.yml
  format: yaml
  label: Kore.ai Conversation API
  slug: koreai-conversation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koreai/refs/heads/main/openapi/koreai-conversation-api-openapi.yml
- filename: koreai-workflows-api-openapi.yml
  format: yaml
  label: Kore.ai Workflows API
  slug: koreai-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koreai/refs/heads/main/openapi/koreai-workflows-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Koreai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kore.ai declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Kore.ai
provider_slug: koreai
scheme_count: 0
schemes: []
slug: koreai-authentication
source_filename: koreai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: searched\nsource: https://docs.kore.ai/ai-for-service/apis/automation/api-introduction\ndocs:\n- https://docs.kore.ai/ai-for-service/apis/automation/api-introduction\n- https://github.com/Koredotcom/docs-v2/blob/main/agent-platform/drafts/api-reference/index.mdx\nnote: >-\n  Kore.ai runs two API estates with two different auth models. AI for Service (the XO /\n  Automation AI platform on platform.kore.ai) authenticates with a signed JWT minted from\n  a JWT App's Client ID + Secret and passed in a non-standard `auth` header. The Agent\n  Platform (Artemis, on agents.kore.ai) authenticates with bearer JWTs or prefixed API\n  keys. Both are documented publicly; neither uses OAuth 2.0 for inbound API access, so\n  there is no OAuth scope surface to capture in scopes/.\nestates:\n- name: AI for Service platform APIs\n  host: https://platform.kore.ai\n  schemes:\n  - id: jwt-app\n    type: apiKey\n    in: header\n    name: auth\n    description:\
  \ >-\n      A JWT signed with the JWT App's Client Secret, carrying the Client ID. Created under\n      App Settings > Dev Tools > Web/Mobile SDK, or in the Admin Console under\n      Security & Control > API Scopes > Manage Apps.\n    signing_algorithms_configurable: true\n    options:\n    - id: enforce-jti\n      description: When enabled, the platform only accepts requests carrying a JTI (JWT ID) claim and rejects the rest.\n    - id: enforce-jwe\n      description: JWE encryption of the token.\n    - id: payload-encryption\n      description: >-\n        AES-256 encryption of request and response payloads. The client supplies a public\n        key; the platform generates an AES-256 key, encrypts the payload with it, and\n        returns the AES key wrapped with the client's public key. Supported on a named\n        subset of endpoints (session history, analytics, conversation details, LLM usage\n        logs, and the user/role admin endpoints).\n  authorization_model:\n    style:\
  \ assigned-scopes\n    description: >-\n      Access is not a single flat key. Each JWT App is assigned API scopes in two\n      namespaces — Platform API Scopes (App Builder features) and Admin Console API Scopes\n      (account administration). The provider publishes a per-API scope matrix: every row of\n      the Automation AI, Contact Center AI, Agent AI, Quality AI and Case Management API\n      lists names the Platform Scope and Admin Console Scope required.\n    reference: https://docs.kore.ai/ai-for-service/apis/api-list\n- name: Agent Platform (Artemis) runtime + management APIs\n  host: https://agents.kore.ai\n  schemes:\n  - id: jwt-bearer\n    type: http\n    scheme: bearer\n    in: header\n    name: Authorization\n    description: JWT bearer token issued after user login.\n  - id: api-key-bearer\n    type: http\n    scheme: bearer\n    in: header\n    name: Authorization\n    description: Long-lived API key prefixed `abl_`, passed as a bearer token.\n    key_prefix: abl_\n\
  \  - id: api-key-header\n    type: apiKey\n    in: header\n    name: X-API-Key\n    description: Service-to-service API key header. Also accepts an origin-restricted public widget key.\n    key_prefix: ak_\n  - id: public-widget-key\n    type: apiKey\n    in: header\n    name: X-Public-Key\n    description: >-\n      Origin-restricted public key, safe in client-side code, exchanged on\n      POST /api/v1/sdk/init for a short-lived SDK session token. Scoped to one project;\n      the runtime validates the Origin header on every SDK request against a configured\n      allowedOrigins list.\n    key_prefix: pk_\n  - id: sdk-session-token\n    type: apiKey\n    in: header\n    name: X-SDK-Token\n    description: Short-lived token for embedded widget sessions.\n    key_prefix: sdk_\n  - id: callback-signature\n    type: http\n    scheme: hmac\n    in: header\n    name: x-callback-signature\n    description: >-\n      HMAC-SHA256 of the request body keyed on the suspension's callback secret,\
  \ formatted\n      `sha256=<hex>`. Verifies inbound human-task/tool callbacks; a failed verification\n      returns 401.\n  spec_declared:\n    file: openapi/koreai-abl-runtime-conversation-openapi.json\n    scheme: ApiKeyAuth (apiKey, header, x-api-key)\n    note: >-\n      The three published specs declare only the x-api-key apiKey scheme. The provider's\n      own API reference documents five more credential types; the spec is thinner than the\n      prose, which is why this artifact is method searched rather than derived.\noauth2: false\nopenid_connect: false\nmtls: false\nsso_for_platform_users:\n  supported: true\n  note: SSO, RBAC and MFA for platform (human) users are listed on the Kore.ai trust center. This is console access, not API authentication.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/koreai/refs/heads/main/authentication/koreai-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Artificial Intelligence
- Conversational AI
- Agents
- Agent Platform
- Contact Center
- Customer Experience
- Employee Experience
- Voice
- Automation
- Model Context Protocol
- Enterprise Software
---
