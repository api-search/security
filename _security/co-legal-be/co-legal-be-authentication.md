---
anonymous_access: true
api_key_in:
- header
auth_types:
- none
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Co Legal Be Authentication
name_suffix: Authentication
oauth_flows: []
overview: Co-Legal secures its APIs with none, apiKey, and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Co-Legal
provider_slug: co-legal-be
scheme_count: 3
schemes:
- description: 'Declared explicitly — the A2A card''s securityRequirements is [{}, {apiKeyAuth: []}, {httpBearer: []}] and the answer_legal_question skill''s own securityRequirements starts with {}. Live probes confirmed: MCP initialize and tools/list, and A2A tasks/list, all succeeded with no credential, and the response carried X-RateLimit-Tier: anon.'
  name: anonymous
  quota: RateLimit-Limit 120 (burst) observed; 600 questions per hour per IP per the agent landing page.
  sources:
  - a2a/co-legal-be-agent-card.json
  - POST https://agent.co-legal.be/mcp (2026-09-19)
  - POST https://agent.co-legal.be/a2a/jsonrpc (2026-09-19)
  type: none
- description: Optional API key for higher rate limits, sent as the x-api-key header. Anonymous callers are accepted within the per-IP cap. (Card securitySchemes.apiKeyAuth.apiKeySecurityScheme.)
  in: header
  issuance:
    contacts:
    - ops@co-legal.be
    - contact@co-legal.be
    cost: null
    method: email request
    note: The 401 on the extended card says "contact ops@co-legal.be to request a key"; the JSON-RPC variant says contact@co-legal.be. payment-options.json shows registrationRequired false for the free tier and a not-yet-available Stripe "pro" subscription of 1000 calls/month, so the key is currently a manually issued quota credential rather than a purchased one.
    self_serve: false
  name: apiKeyAuth
  optional: true
  parameter: x-api-key
  sources:
  - a2a/co-legal-be-agent-card.json
  - https://co-legal.be/llms.txt
  storage: Hashed at rest — "Optionele API keys worden gehasht opgeslagen — wij bewaren nooit de plaintext" (https://co-legal.be/legal).
  type: apiKey
  unlocks:
  - higher fair-use quota
  - agent/getAuthenticatedExtendedCard and GET /extendedAgentCard (paid skills)
- description: 'The same optional API key presented as Authorization: Bearer <key> (RFC 6750). (Card securitySchemes.httpBearer.httpAuthSecurityScheme.)'
  name: httpBearer
  note: Opaque key, not an OAuth access token; bearerFormat is not declared.
  optional: true
  scheme: bearer
  sources:
  - a2a/co-legal-be-agent-card.json
  - https://agent.co-legal.be/llms.txt
  type: http
slug: co-legal-be-authentication
source_filename: co-legal-be-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://agent.co-legal.be/.well-known/agent-card.json\nderived_from:\n- a2a/co-legal-be-agent-card.json\n- mcp/co-legal-be-mcp-initialize.json\ndocs:\n- https://co-legal.be/llms.txt\n- https://agent.co-legal.be/llms.txt\n- https://agent.co-legal.be/\n- https://co-legal.be/legal\nsummary:\n  types: [none, apiKey, http]\n  api_key_in: [header]\n  oauth2_flows: []\n  bearer: true\n  anonymous_access: true\n  credential_classes: 1\n  headline: >-\n    Anonymous by design. Both agent surfaces — the A2A JSON-RPC endpoint and the MCP server — accept\n    unauthenticated callers within a per-IP fair-use quota; the card declares this as a first-class option\n    (securityRequirements[0] = {}). ONE optional credential exists, an API key, presentable either as the\n    x-api-key header or as Authorization: Bearer <key> (RFC 6750). It raises the rate-limit quota and unlocks\n    the extended agent card (paid skills); it is obtained by\
  \ email, not self-serve, and the provider states keys\n    are stored hashed. No OAuth 2.0, no OIDC, no discovery documents, no scopes. The card itself is\n    authenticated the other way round — it is JWS-signed (ES256) and verifiable against a published JWKS.\nschemes:\n- name: anonymous\n  type: none\n  description: >-\n    Declared explicitly — the A2A card's securityRequirements is [{}, {apiKeyAuth: []}, {httpBearer: []}] and\n    the answer_legal_question skill's own securityRequirements starts with {}. Live probes confirmed: MCP\n    initialize and tools/list, and A2A tasks/list, all succeeded with no credential, and the response carried\n    X-RateLimit-Tier: anon.\n  quota: RateLimit-Limit 120 (burst) observed; 600 questions per hour per IP per the agent landing page.\n  sources: [a2a/co-legal-be-agent-card.json, 'POST https://agent.co-legal.be/mcp (2026-09-19)', 'POST https://agent.co-legal.be/a2a/jsonrpc (2026-09-19)']\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter:\
  \ x-api-key\n  optional: true\n  description: Optional API key for higher rate limits, sent as the x-api-key header. Anonymous callers are accepted within the per-IP cap. (Card securitySchemes.apiKeyAuth.apiKeySecurityScheme.)\n  issuance:\n    method: email request\n    contacts: [ops@co-legal.be, contact@co-legal.be]\n    self_serve: false\n    cost: null\n    note: 'The 401 on the extended card says \"contact ops@co-legal.be to request a key\"; the JSON-RPC variant says contact@co-legal.be. payment-options.json shows registrationRequired false for the free tier and a not-yet-available Stripe \"pro\" subscription of 1000 calls/month, so the key is currently a manually issued quota credential rather than a purchased one.'\n  storage: 'Hashed at rest — \"Optionele API keys worden gehasht opgeslagen — wij bewaren nooit de plaintext\" (https://co-legal.be/legal).'\n  unlocks: [higher fair-use quota, 'agent/getAuthenticatedExtendedCard and GET /extendedAgentCard (paid skills)']\n  sources:\
  \ [a2a/co-legal-be-agent-card.json, 'https://co-legal.be/llms.txt']\n- name: httpBearer\n  type: http\n  scheme: bearer\n  optional: true\n  description: 'The same optional API key presented as Authorization: Bearer <key> (RFC 6750). (Card securitySchemes.httpBearer.httpAuthSecurityScheme.)'\n  note: Opaque key, not an OAuth access token; bearerFormat is not declared.\n  sources: [a2a/co-legal-be-agent-card.json, 'https://agent.co-legal.be/llms.txt']\nmcp_server:\n  endpoint: https://agent.co-legal.be/mcp\n  auth: none required; the same optional x-api-key applies per payment-options.json (mcpEndpoint under the free tier)\n  oauth_metadata: none — /.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource both 404 on the resource host\n  session: stateless; no Mcp-Session-Id issued\ncard_integrity:\n  signature: JWS ES256, kid colegal-agent-es256-1, jku https://agent.co-legal.be/.well-known/jwks.json, typ JOSE\n  verified: '2026-09-19 — see a2a/co-legal-be-a2a.yml\
  \ x-evidence.signature_verification'\n  note: Verifying the card signature lets a client establish that the endpoint, skills and schemes it is about to trust were published by the key holder, independent of TLS. Few catalog cards offer this.\ndelegated_identity: false\ndynamic_client_registration: false\nprotected_resource_metadata: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/co-legal-be/refs/heads/main/authentication/co-legal-be-authentication.yml
summary_line: none/apiKey/http · 3 schemes
tags:
- Legal
- Legal Research
- Tax
- Case Law
- Legislation
- Company Registry
- VAT Validation
- Belgium
- Netherlands
- European Union
- A2A
- MCP
- Agent-Native
- Artificial Intelligence
- Legal Tech
---
