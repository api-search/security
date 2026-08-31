---
api_key_in:
- header
api_specs:
- filename: replyrai-accounts-api-openapi.yml
  format: yaml
  label: Replyr.ai Accounts API
  slug: replyrai-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replyrai/refs/heads/main/openapi/replyrai-accounts-api-openapi.yml
- filename: replyrai-ai-agents-api-openapi.yml
  format: yaml
  label: Replyr.ai AI Agents API
  slug: replyrai-ai-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replyrai/refs/heads/main/openapi/replyrai-ai-agents-api-openapi.yml
- filename: replyrai-appointment-management-api-openapi.yml
  format: yaml
  label: Replyr.ai Appointment Management API
  slug: replyrai-appointment-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replyrai/refs/heads/main/openapi/replyrai-appointment-management-api-openapi.yml
- filename: replyrai-contacts-api-openapi.yml
  format: yaml
  label: Replyr.ai Contacts API
  slug: replyrai-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replyrai/refs/heads/main/openapi/replyrai-contacts-api-openapi.yml
- filename: replyrai-ecommerce-api-openapi.yml
  format: yaml
  label: Replyr.ai Ecommerce API
  slug: replyrai-ecommerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replyrai/refs/heads/main/openapi/replyrai-ecommerce-api-openapi.yml
- filename: replyrai-pipelines-api-openapi.yml
  format: yaml
  label: Replyr.ai Pipelines API
  slug: replyrai-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replyrai/refs/heads/main/openapi/replyrai-pipelines-api-openapi.yml
- filename: replyrai-templates-api-openapi.yml
  format: yaml
  label: Replyr.ai Templates API
  slug: replyrai-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replyrai/refs/heads/main/openapi/replyrai-templates-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Replyrai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Replyr.ai secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Replyr.ai
provider_slug: replyrai
scheme_count: 1
schemes:
- applied: global
  expiry: not published
  in: header
  issuance: From the Replyr operator console at https://app.replyr.ai. Not documented in the reference; there is no self-serve sign-up route (https://app.replyr.ai/en/register returns 404), so a key follows a sales conversation.
  name: APIKeyHeader
  operations_covered: 65
  parameter: X-ACCESS-TOKEN
  revocation_policy: not published
  rotation_policy: not published
  sources:
  - openapi/replyrai-platform-api-swagger.json
  type: apiKey
slug: replyrai-authentication
source_filename: replyrai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/replyrai-platform-api-swagger.json\ndocs: https://app.replyr.ai/api\nnote: >-\n  Baseline derived by derive-authentication.py from the provider's Swagger 2.0\n  securityDefinitions, then upgraded with the live behaviour observed against\n  https://app.replyr.ai/api/accounts/me on 2026-08-13. Replyr publishes no prose\n  authentication guide - the Swagger UI at https://app.replyr.ai/api is the whole\n  reference - so token issuance, rotation and revocation are undocumented.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  scopes: none\n  multi_factor: false\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-ACCESS-TOKEN\n  applied: global\n  operations_covered: 65\n  issuance: >-\n    From the Replyr operator console at https://app.replyr.ai. Not documented in\n    the reference; there is no self-serve sign-up route\n\
  \    (https://app.replyr.ai/en/register returns 404), so a key follows a sales\n    conversation.\n  rotation_policy: not published\n  revocation_policy: not published\n  expiry: not published\n  sources:\n  - openapi/replyrai-platform-api-swagger.json\nauthorization:\n  model: all-or-nothing\n  scopes: []\n  detail: >-\n    There is no scope, permission or role surface on the API. One account key\n    authorizes all 65 operations, including operations with external\n    consequences - sending messages to real end users on WhatsApp and other\n    channels (sendTextMessage, sendFile, sendFlowToUser, sendContent,\n    sendProduct), deleting pipeline data (pipelinesDeleteCard), and changing\n    order payment state (payOrder, changeOrder). A key issued for a read-only\n    integration cannot be restricted to reads.\n  tenancy: >-\n    Keys are account-scoped. page_id on Account, Contact, Cart and Order is the\n    tenant key; the API exposes no cross-account operation.\nfailure_behavior:\n\
  \  status: 401\n  body: '{\"error\":{\"code\":401,\"message\":\"No valid API key provided.\"}}'\n  content_type: text/html; charset=UTF-8\n  www_authenticate_header: false\n  detail: >-\n    Identical response for a missing header, a malformed token and a\n    syntactically valid but invalid token - the three cases cannot be\n    distinguished by a client. The same 401 is also returned for /api/* paths\n    that do not exist, so a 401 does not confirm an operation exists. No\n    WWW-Authenticate challenge header is sent, so the response is not\n    self-describing to a generic HTTP client.\ntransport:\n  https_required: true\n  tls_version: TLSv1.3\n  hsts: false\n  hsts_detail: >-\n    app.replyr.ai - the host carrying both the API and the authenticated console -\n    does not send Strict-Transport-Security, though the marketing host replyr.ai\n    does. See security/replyrai-domain-security.yml.\ndiscovery:\n  openid_configuration: 404\n  oauth_authorization_server: 404\n  oauth_protected_resource:\
  \ 404\n  detail: See well-known/replyrai-well-known.yml - 16 paths probed, 0 documents.\nx-evidence:\n  fetched: '2026-08-13'\n  probes:\n  - url: https://app.replyr.ai/api/accounts/me\n    request: no auth header\n    status: 401\n  - url: https://app.replyr.ai/api/accounts/me\n    request: X-ACCESS-TOKEN with an invalid value\n    status: 401\n    note: Identical body to the no-header case.\n  - url: https://app.replyr.ai/api\n    status: 200\n    note: Swagger UI reference page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/replyrai/refs/heads/main/authentication/replyrai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Chatbots
- Conversational AI
- Customer Engagement
- Lead Generation
- WhatsApp
- Marketing
- Messaging
- CRM
- Appointment Scheduling
- Healthcare
- Malaysia
---
