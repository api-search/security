---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Sursatech Com Authentication
name_suffix: Authentication
oauth_flows:
- client_credentials (anonymous — token_endpoint_auth_methods_supported [none])
overview: SursaTech secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the client_credentials (anonymous — token_endpoint_auth_methods_supported [none]) flow(s).
provider_name: SursaTech
provider_slug: sursatech-com
scheme_count: 1
schemes:
- applies_to: every JSON-RPC method on POST https://api.sursatech.com/api/a2a (the card declares security [bearerAuth] at the card level with no per-skill override)
  bearerFormat: opaque
  description: Opaque bearer token returned by /api/a2a/register or /api/a2a/token, or minted out-of-band for known partners.
  header: 'Authorization: Bearer <accessToken>'
  name: bearerAuth
  scheme: bearer
  sources:
  - a2a/sursatech-com-agent-card.json#securitySchemes.bearerAuth
  - https://api.sursatech.com/auth.md ("Credential Use")
  type: http
slug: sursatech-com-authentication
source_filename: sursatech-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://api.sursatech.com/auth.md (saved verbatim at authentication/sursatech-com-auth.md), the agent card securitySchemes/security (a2a/sursatech-com-agent-card.json), the RFC 8414 / OIDC / RFC 9728 discovery documents in well-known/, and live anonymous probes of the endpoints on 2026-09-19.\ndocs: https://api.sursatech.com/auth.md\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  oauth2_flows:\n  - client_credentials (anonymous — token_endpoint_auth_methods_supported [none])\n  registration: anonymous dynamic self-registration (RFC 7591-style registration_endpoint, non-standard response shape)\n  api_key_in: []\n  openapi: none — no OpenAPI is served (the api-catalog advertises https://api.sursatech.com/openapi.json, which 404s), so this profile is searched from the docs and discovery metadata rather than derived from a spec\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: opaque\n\
  \  description: Opaque bearer token returned by /api/a2a/register or /api/a2a/token, or minted out-of-band for known partners.\n  header: 'Authorization: Bearer <accessToken>'\n  applies_to: every JSON-RPC method on POST https://api.sursatech.com/api/a2a (the card declares security [bearerAuth] at the card level with no per-skill override)\n  sources:\n  - a2a/sursatech-com-agent-card.json#securitySchemes.bearerAuth\n  - https://api.sursatech.com/auth.md (\"Credential Use\")\nauthorization_server:\n  issuer: https://api.sursatech.com\n  metadata:\n  - https://api.sursatech.com/.well-known/oauth-authorization-server\n  - https://api.sursatech.com/.well-known/openid-configuration\n  - https://www.sursatech.com/.well-known/oauth-authorization-server (same content)\n  registration_endpoint: https://api.sursatech.com/api/a2a/register\n  token_endpoint: https://api.sursatech.com/api/a2a/token\n  authorization_endpoint: https://api.sursatech.com/auth.md\n  authorization_endpoint_note: The \"\
  authorization endpoint\" is a markdown document, not an interactive grant UI — there is no user-facing authorization step; response_types_supported is [\"none\"].\n  jwks_uri: https://api.sursatech.com/.well-known/jwks.json\n  jwks_note: '{\"keys\":[]} — empty; tokens are opaque, not JWTs, so there is nothing to verify offline and no token introspection endpoint is published.'\n  grant_types_supported:\n  - client_credentials\n  token_endpoint_auth_methods_supported:\n  - none\n  scopes_supported:\n  - a2a\n  - company.read\n  - requirements.write\n  - booking.write\n  agent_auth:\n    note: A non-standard extension block in the RFC 8414 document describing agent registration.\n    identity_types_supported:\n    - anonymous\n    credential_types_supported:\n    - access_token\n    - bearer\n    register_uri: https://api.sursatech.com/api/a2a/register\n    claim_uri: https://api.sursatech.com/api/a2a/register\n    not_supported: ID-JAG identity assertions and user-claimed service-auth ceremonies\
  \ (auth.md, \"Registration\")\nprotected_resources:\n- resource: https://api.sursatech.com/api/a2a\n  metadata: https://api.sursatech.com/.well-known/oauth-protected-resource\n  bearer_methods_supported: [header]\n  challenge: 'WWW-Authenticate: Bearer realm=\"SursaTech A2A\", resource_metadata=\"https://api.sursatech.com/.well-known/oauth-protected-resource\" (observed on an anonymous POST, HTTP 401 {\"detail\":\"Missing bearer token\"})'\n- resource: https://www.sursatech.com\n  metadata: https://www.sursatech.com/.well-known/oauth-protected-resource\n  note: the website origin declares itself a protected resource of the same authorization server; the API resource document on api.sursatech.com is the operative one for the A2A endpoint\nflows:\n- name: Anonymous self-registration\n  documented_at: https://api.sursatech.com/auth.md\n  steps:\n  - 'POST https://api.sursatech.com/api/a2a/register with Content-Type: application/json and body {\"name\": \"Your agent name\"}'\n  - 'Response\
  \ (per auth.md): tokenType \"Bearer\" and accessToken; observed response fields on 2026-09-19: clientId (UUID), name, tokenType, accessToken, rateLimitPerMinute (60). An EMPTY body is accepted and a default name is assigned.'\n  - The plaintext token is returned only once; store it securely.\n  - 'Send Authorization: Bearer <accessToken> on POST https://api.sursatech.com/api/a2a'\n  token_scope: self-registration tokens receive the A2A agent scope (a2a) and are rate-limited per client and per IP\n- name: Token endpoint\n  documented_at: https://api.sursatech.com/.well-known/oauth-authorization-server (token_endpoint) and the card's x-sursatech-tokenUrl\n  steps:\n  - 'POST https://api.sursatech.com/api/a2a/token — observed on 2026-09-19 to answer an anonymous EMPTY JSON body with HTTP 200 {access_token, token_type \"Bearer\", scope \"a2a\", client_id} (RFC 6749 §5.1 field names, unlike /register)'\n  note: auth.md does not document the token endpoint's request shape; the discovery metadata\
  \ lists client_credentials with auth method none, and the empty-body probe confirms no client credential is required to mint an a2a-scoped token.\n- name: Partner credentials\n  documented_at: a2a/sursatech-com-agent-card.json#securitySchemes.bearerAuth.description\n  note: tokens \"minted out-of-band for known partners\" — no public flow; presumably the path to company.read / requirements.write / booking.write scopes beyond the default a2a scope\nrevocation:\n  self_service: false\n  note: 'auth.md: \"There is no self-service revocation endpoint yet. Contact info@sursatech.com to disable a registered agent credential.\"'\n  contact: info@sursatech.com\nerror_behaviour:\n  missing_token:\n    status: 401\n    body: '{\"detail\":\"Missing bearer token\"}'\n    headers:\n      www-authenticate: Bearer realm=\"SursaTech A2A\", resource_metadata=\"https://api.sursatech.com/.well-known/oauth-protected-resource\"\n  note: The unauthenticated challenge fires before JSON-RPC method dispatch for\
  \ the A2A 1.0 method names (SendMessage, GetTask); unknown method names return JSON-RPC -32601 with HTTP 200 without an auth check.\nprovenance_note: 'This profile used no credential: it records the anonymous probes only. The tokens the empty-body probes returned were discarded and never sent to the API.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sursatech-com/refs/heads/main/authentication/sursatech-com-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Agents
- A2A
- Agent-to-Agent
- AI Consulting
- Product Engineering
- Software Development
- RAG
- QA Automation
- Nepal
- agent-native
- Company
---
