---
api_key_in:
- header
- query
api_specs:
- filename: builtwith-live-feed-asyncapi.yml
  format: yaml
  label: BuiltWith Live Feed API
  slug: builtwith-live-feed-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/asyncapi/builtwith-live-feed-asyncapi.yml
- filename: builtwith-agent-stripe-topup-openapi.json
  format: json
  label: BuiltWith Agent Payment API
  slug: builtwith-agent-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-agent-stripe-topup-openapi.json
- filename: builtwith-rest-api-openapi.json
  format: json
  label: BuiltWith REST API
  slug: builtwith-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-rest-api-openapi.json
- filename: builtwith-x402-pay-per-call-openapi.json
  format: json
  label: BuiltWith x402 Pay-per-Call API
  slug: builtwith-x402-pay-per-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-x402-pay-per-call-openapi.json
- filename: builtwith-bulk-processing-api-openapi.yml
  format: yaml
  label: BuiltWith Bulk Processing API
  slug: builtwith-bulk-processing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-bulk-processing-api-openapi.yml
- filename: builtwith-domain-lookup-api-openapi.yml
  format: yaml
  label: BuiltWith Domain Lookup API
  slug: builtwith-domain-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-domain-lookup-api-openapi.yml
- filename: builtwith-domain-relationships-api-openapi.yml
  format: yaml
  label: BuiltWith Domain Relationships API
  slug: builtwith-domain-relationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-domain-relationships-api-openapi.yml
- filename: builtwith-free-lookup-api-openapi.yml
  format: yaml
  label: BuiltWith Free Lookup API
  slug: builtwith-free-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-free-lookup-api-openapi.yml
- filename: builtwith-tag-lookup-api-openapi.yml
  format: yaml
  label: BuiltWith Tag Lookup API
  slug: builtwith-tag-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-tag-lookup-api-openapi.yml
- filename: builtwith-technology-changes-api-openapi.yml
  format: yaml
  label: BuiltWith Technology Changes API
  slug: builtwith-technology-changes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-technology-changes-api-openapi.yml
- filename: builtwith-technology-lists-api-openapi.yml
  format: yaml
  label: BuiltWith Technology Lists API
  slug: builtwith-technology-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-technology-lists-api-openapi.yml
- filename: builtwith-technology-trends-api-openapi.yml
  format: yaml
  label: BuiltWith Technology Trends API
  slug: builtwith-technology-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-technology-trends-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Builtwith Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: BuiltWith secures its APIs with apiKey, http, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: BuiltWith
provider_slug: builtwith
scheme_count: 5
schemes:
- applies_to: all REST intelligence endpoints
  format: 'Authorization: API {guid}'
  in: header
  name: apiKeyHeader
  parameter: Authorization
  preferred: true
  sources:
  - https://api.builtwith.com/domain-api
  - openapi/builtwith-rest-api-openapi.json
  - openapi/builtwith-bulk-processing-api-openapi.yml
  - openapi/builtwith-domain-lookup-api-openapi.yml
  - openapi/builtwith-domain-relationships-api-openapi.yml
  - openapi/builtwith-free-lookup-api-openapi.yml
  - openapi/builtwith-tag-lookup-api-openapi.yml
  - openapi/builtwith-technology-changes-api-openapi.yml
  - openapi/builtwith-technology-lists-api-openapi.yml
  - openapi/builtwith-technology-trends-api-openapi.yml
  type: apiKey
- applies_to: all REST intelligence endpoints and the WebSocket Live Feed
  format: GUID (UUID v4), or a bw- prefixed device token
  in: query
  name: apiKeyQuery
  note: Retained for compatibility. Deprecated on the Stripe credit top-up service only.
  parameter: KEY
  sources:
  - https://api.builtwith.com/domain-api
  - openapi/builtwith-rest-api-openapi.json
  - openapi/builtwith-bulk-processing-api-openapi.yml
  - openapi/builtwith-domain-lookup-api-openapi.yml
  - openapi/builtwith-domain-relationships-api-openapi.yml
  - openapi/builtwith-free-lookup-api-openapi.yml
  - openapi/builtwith-tag-lookup-api-openapi.yml
  - openapi/builtwith-technology-changes-api-openapi.yml
  - openapi/builtwith-technology-lists-api-openapi.yml
  - openapi/builtwith-technology-trends-api-openapi.yml
  type: apiKey
- applies_to: https://api.builtwith.com/mcp (hosted MCP server) and the local stdio server
  format: 'Authorization: Bearer {builtwith-api-key}'
  name: mcpBearer
  note: Bring-your-own BuiltWith API key. tools/list and initialize answer anonymously; tool invocation requires the bearer key or an x402 creditKey.
  scheme: bearer
  sources:
  - https://builtwith.com/.well-known/mcp.json
  - https://builtwith.com/.well-known/agent-card.json
  type: http
- applies_to: https://payments.builtwith.com/v1/billing/* and the https://api.builtwith.com/mppx/* aliases
  format: 'Authorization: Bearer {agent-billing-key}'
  name: agentBillingKey
  note: Separately scoped credential obtained from https://payments.builtwith.com/agent-payment-api-config. General API keys and temporary bw- tokens cannot purchase credits.
  scheme: bearer
  sources:
  - openapi/builtwith-agent-stripe-topup-openapi.json
  - openapi/builtwith-rest-api-openapi.json
  type: http
- discovery:
  - https://api.builtwith.com/.well-known/oauth-authorization-server
  - https://api.builtwith.com/.well-known/oauth-protected-resource
  flows:
  - authorizationUrl: https://api.builtwith.com/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    registrationUrl: https://api.builtwith.com/oauth/register
    scopes:
    - api.read
    - api.write
    tokenUrl: https://api.builtwith.com/token
    token_endpoint_auth_methods:
    - none
  name: oauth2
  note: Not declared in any OpenAPI - published only as RFC 8414 / RFC 9728 discovery documents, which is the shape an MCP client negotiates. Detail in scopes/builtwith-scopes.yml.
  sources:
  - https://api.builtwith.com/.well-known/oauth-authorization-server
  type: oauth2
slug: builtwith-authentication
source_filename: builtwith-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\ndocs: https://api.builtwith.com/domain-api\nsource: >-\n  https://api.builtwith.com/domain-api, https://api.builtwith.com/llms.txt,\n  https://api.builtwith.com/.well-known/oauth-authorization-server,\n  https://api.builtwith.com/.well-known/oauth-protected-resource,\n  https://builtwith.com/.well-known/agent-card.json,\n  openapi/builtwith-rest-api-openapi.json, openapi/builtwith-agent-stripe-topup-openapi.json,\n  openapi/builtwith-domain-lookup-api-openapi.yml and the six sibling refined specs\nsummary:\n  types: [apiKey, http, oauth2]\n  api_key_in: [header, query]\n  oauth2_flows: [authorizationCode]\n  pkce: S256\n  dynamic_client_registration: true\n  preferred: 'Authorization: API {key}'\n  https_only: true\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Authorization: API {guid}'\n  preferred: true\n  applies_to: all REST intelligence endpoints\n  sources:\n  - https://api.builtwith.com/domain-api\n\
  \  - openapi/builtwith-rest-api-openapi.json\n  - openapi/builtwith-bulk-processing-api-openapi.yml\n  - openapi/builtwith-domain-lookup-api-openapi.yml\n  - openapi/builtwith-domain-relationships-api-openapi.yml\n  - openapi/builtwith-free-lookup-api-openapi.yml\n  - openapi/builtwith-tag-lookup-api-openapi.yml\n  - openapi/builtwith-technology-changes-api-openapi.yml\n  - openapi/builtwith-technology-lists-api-openapi.yml\n  - openapi/builtwith-technology-trends-api-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: KEY\n  format: GUID (UUID v4), or a bw- prefixed device token\n  applies_to: all REST intelligence endpoints and the WebSocket Live Feed\n  note: 'Retained for compatibility. Deprecated on the Stripe credit top-up service only.'\n  sources:\n  - https://api.builtwith.com/domain-api\n  - openapi/builtwith-rest-api-openapi.json\n  - openapi/builtwith-bulk-processing-api-openapi.yml\n  - openapi/builtwith-domain-lookup-api-openapi.yml\n  - openapi/builtwith-domain-relationships-api-openapi.yml\n\
  \  - openapi/builtwith-free-lookup-api-openapi.yml\n  - openapi/builtwith-tag-lookup-api-openapi.yml\n  - openapi/builtwith-technology-changes-api-openapi.yml\n  - openapi/builtwith-technology-lists-api-openapi.yml\n  - openapi/builtwith-technology-trends-api-openapi.yml\n- name: mcpBearer\n  type: http\n  scheme: bearer\n  format: 'Authorization: Bearer {builtwith-api-key}'\n  applies_to: https://api.builtwith.com/mcp (hosted MCP server) and the local stdio server\n  note: >-\n    Bring-your-own BuiltWith API key. tools/list and initialize answer anonymously; tool\n    invocation requires the bearer key or an x402 creditKey.\n  sources:\n  - https://builtwith.com/.well-known/mcp.json\n  - https://builtwith.com/.well-known/agent-card.json\n- name: agentBillingKey\n  type: http\n  scheme: bearer\n  format: 'Authorization: Bearer {agent-billing-key}'\n  applies_to: https://payments.builtwith.com/v1/billing/* and the https://api.builtwith.com/mppx/* aliases\n  note: >-\n    Separately scoped\
  \ credential obtained from\n    https://payments.builtwith.com/agent-payment-api-config. General API keys and temporary\n    bw- tokens cannot purchase credits.\n  sources:\n  - openapi/builtwith-agent-stripe-topup-openapi.json\n  - openapi/builtwith-rest-api-openapi.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.builtwith.com/authorize\n    tokenUrl: https://api.builtwith.com/token\n    registrationUrl: https://api.builtwith.com/oauth/register\n    code_challenge_methods: [S256]\n    token_endpoint_auth_methods: [none]\n    scopes: [api.read, api.write]\n  discovery:\n  - https://api.builtwith.com/.well-known/oauth-authorization-server\n  - https://api.builtwith.com/.well-known/oauth-protected-resource\n  note: >-\n    Not declared in any OpenAPI - published only as RFC 8414 / RFC 9728 discovery documents,\n    which is the shape an MCP client negotiates. Detail in scopes/builtwith-scopes.yml.\n  sources:\n  - https://api.builtwith.com/.well-known/oauth-authorization-server\n\
  device_code_authorization:\n  purpose: Lets an agent obtain a temporary token without asking a human to paste an API key.\n  start: POST https://api.builtwith.com/agent-auth/start\n  verification_uri_template: https://api.builtwith.com/device-auth?code={device_code}\n  poll: POST https://api.builtwith.com/agent-auth/token\n  poll_body: '{\"device_code\":\"<device_code>\"}'\n  default_interval_seconds: 5\n  code_expires_in_seconds: 900\n  token_prefix: bw-\n  token_type: bearer\n  token_expires_in_seconds: 86400\n  pending_responses: [authorization_pending, access_denied, expired_token]\n  error_status: 400\n  usage: 'Pass the returned token as KEY=bw-... exactly like a permanent key.'\n  operations:\n  - openapi/builtwith-rest-api-openapi.json#agent_auth_start\n  - openapi/builtwith-rest-api-openapi.json#agent_auth_token\n  source: https://api.builtwith.com/llms.txt\npayment_credentials:\n- name: creditKey\n  protocol: x402 v2\n  description: Reusable, non-expiring prepaid lookup-unit\
  \ key bought with Base USDC; held in a separate x402 ledger, not a BuiltWith account.\n  bound_to: the payer wallet that created it\n  discovery: https://api.builtwith.com/.well-known/x402\n- name: passToken\n  protocol: x402 v2\n  description: 30-day Basic or Pro List pass token required for x402 List and Keyword Search tools.\nintrospection:\n  whoami: GET https://api.builtwith.com/whoamiv1/api.json\n  usage: GET https://api.builtwith.com/usagev2/api.json\n  note: Both are free (no credits) and let an agent discover its own plan, limits, credit costs and privacy flags before acting.\nkey_handling:\n  rotation: via the account dashboard\n  guidance:\n  - HTTPS is required on every endpoint.\n  - Never expose the API key in client-side code.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/authentication/builtwith-authentication.yml
summary_line: apiKey/http/oauth2 · 5 schemes
tags:
- Technology Profiling
- Lead Generation
- Web Intelligence
- Technology Detection
- Website Analysis
- Market Research
- Technographics
- Sales Intelligence
- AI Agents
- MCP
- Agentic Commerce
- Real-Time Data
---
