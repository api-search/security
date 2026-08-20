---
api_key_in:
- header
api_specs:
- filename: regal-reporting-webhooks-asyncapi.yml
  format: yaml
  label: Regal Reporting Webhooks
  slug: regal-reporting-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/asyncapi/regal-reporting-webhooks-asyncapi.yml
- filename: regal-ai-branded-phone-numbers-api-openapi.yml
  format: yaml
  label: Regal Branded Phone Numbers API
  slug: regal-ai-branded-phone-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/openapi/regal-ai-branded-phone-numbers-api-openapi.yml
- filename: regal-ai-business-profiles-api-openapi.yml
  format: yaml
  label: Regal Business Profiles API
  slug: regal-ai-business-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/openapi/regal-ai-business-profiles-api-openapi.yml
- filename: regal-ai-campaigns-api-openapi.yml
  format: yaml
  label: Regal Campaigns API
  slug: regal-ai-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/openapi/regal-ai-campaigns-api-openapi.yml
- filename: regal-ai-dispositions-api-openapi.yml
  format: yaml
  label: Regal Dispositions API
  slug: regal-ai-dispositions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/openapi/regal-ai-dispositions-api-openapi.yml
- filename: regal-ai-events-api-openapi.yml
  format: yaml
  label: Regal Events API
  slug: regal-ai-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/openapi/regal-ai-events-api-openapi.yml
- filename: regal-ai-messages-api-openapi.yml
  format: yaml
  label: Regal Messages API
  slug: regal-ai-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/openapi/regal-ai-messages-api-openapi.yml
- filename: regal-ai-phone-numbers-api-openapi.yml
  format: yaml
  label: Regal Phone Numbers API
  slug: regal-ai-phone-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/openapi/regal-ai-phone-numbers-api-openapi.yml
- filename: regal-ai-users-api-openapi.yml
  format: yaml
  label: Regal Users API
  slug: regal-ai-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/openapi/regal-ai-users-api-openapi.yml
- filename: regal-ai-call-handoffs-api-openapi.yml
  format: yaml
  label: Regal Call Handoffs API
  slug: regal-ai-call-handoffs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/openapi/regal-ai-call-handoffs-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Regal Ai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: Regal secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: Regal
provider_slug: regal-ai
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/regal-ai-branded-phone-numbers-api-openapi.yml
  - openapi/regal-ai-business-profiles-api-openapi.yml
  - openapi/regal-ai-call-handoffs-api-openapi.yml
  - openapi/regal-ai-campaigns-api-openapi.yml
  - openapi/regal-ai-dispositions-api-openapi.yml
  - openapi/regal-ai-events-api-openapi.yml
  - openapi/regal-ai-messages-api-openapi.yml
  - openapi/regal-ai-phone-numbers-api-openapi.yml
  - openapi/regal-ai-users-api-openapi.yml
  type: apiKey
slug: regal-ai-authentication
source_filename: regal-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: openapi/regal-ai-branded-phone-numbers-api-openapi.yml, openapi/regal-ai-business-profiles-api-openapi.yml,\n  openapi/regal-ai-call-handoffs-api-openapi.yml, openapi/regal-ai-campaigns-api-openapi.yml,\n  openapi/regal-ai-dispositions-api-openapi.yml, openapi/regal-ai-events-api-openapi.yml, openapi/regal-ai-messages-api-openapi.yml,\n  openapi/regal-ai-phone-numbers-api-openapi.yml, openapi/regal-ai-users-api-openapi.yml\ndocs: https://developer.regal.ai/reference/overview\nmcp_docs: https://developer.regal.ai/docs/regal-mcp\nissuance: >-\n  API keys are issued by Regal support only — \"For an API key please, reach out to\n  support@regal.ai\". There is no self-serve key page, no key rotation procedure, and no\n  test/live key pair; every documented call goes to production with a production key.\ntransport_note: >-\n  The key is sent RAW in the Authorization header. Regal documents no scheme prefix — not\n  Bearer, not Basic.\
  \ A wrong key returns 403 {\"statusCode\":403,\"message\":\"Invalid API\n  Key\",\"error\":\"Forbidden\"} on the application-layer endpoints and 401\n  {\"message\":\"Unauthorized\"} at the gateway, so both statuses must be treated as auth\n  failures.\noauth:\n  surface: mcp\n  endpoint: https://mcp.regal.ai/v1/external-mcp/mcp\n  type: oauth2\n  identity_provider: Okta\n  flows: [authorizationCode, refreshToken]\n  pkce: S256\n  dynamic_client_registration: true\n  scopes: [openid, profile, email, offline_access]\n  metadata: well-known/regal-ai-oauth-authorization-server.json\n  detail: scopes/regal-ai-scopes.yml\n  note: >-\n    OAuth exists ONLY on the hosted MCP server. None of the REST APIs accept an OAuth\n    token, and the MCP server does not accept an API key.\nsso:\n  saml: [Okta, Google, Azure]\n  scim: Okta\n  docs:\n    - https://developer.regal.ai/docs/okta-sso\n    - https://developer.regal.ai/docs/google-sso\n    - https://developer.regal.ai/docs/azure-sso\n    - https://developer.regal.ai/docs/okta-scim\n\
  \  note: Application/user authentication, not API authentication.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - refreshToken\n  surfaces:\n    rest: apiKey\n    mcp: oauth2\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/regal-ai-branded-phone-numbers-api-openapi.yml\n  - openapi/regal-ai-business-profiles-api-openapi.yml\n  - openapi/regal-ai-call-handoffs-api-openapi.yml\n  - openapi/regal-ai-campaigns-api-openapi.yml\n  - openapi/regal-ai-dispositions-api-openapi.yml\n  - openapi/regal-ai-events-api-openapi.yml\n  - openapi/regal-ai-messages-api-openapi.yml\n  - openapi/regal-ai-phone-numbers-api-openapi.yml\n  - openapi/regal-ai-users-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/authentication/regal-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- AI Agents
- Voice AI
- Contact Center
- Outbound Calling
- Inbound Calling
- Phone Agents
- SMS
- Chat
- WebRTC
- Conversation Intelligence
- Journey Orchestration
- Branded Caller ID
- CCaaS
- CPaaS
- Sales Dialer
- Customer Engagement
---
