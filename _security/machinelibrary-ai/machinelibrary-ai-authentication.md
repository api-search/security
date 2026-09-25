---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: machinelibrary-ai-openapi.yml
  format: yaml
  label: Machine Library API
  slug: machine-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/machinelibrary-ai/refs/heads/main/openapi/machinelibrary-ai-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Machinelibrary Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Space Frontiers secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Space Frontiers
provider_slug: machinelibrary-ai
scheme_count: 3
schemes:
- description: Machine Library API key from https://machinelibrary.ai/keys.
  expiry: Long-lived; does not expire automatically, revocable from account settings (privacy policy section 4).
  in: header
  key_prefix: sf_live_ (example shape in the MCP README and smithery.yaml exampleConfig)
  name: api_key
  parameter: X-Api-Key
  sources:
  - openapi/machinelibrary-ai-openapi.yml
  - openapi/machinelibrary-ai-recognition-openapi.yml
  type: apiKey
- bearerFormat: API key or OAuth 2.0 access token
  description: Send the same API key, or an OAuth 2.0 access token, as a Bearer token.
  name: bearer_auth
  scheme: bearer
  sources:
  - openapi/machinelibrary-ai-openapi.yml
  - openapi/machinelibrary-ai-recognition-openapi.yml
  type: http
- a2a_card_schemes:
    apiKey: header X-Api-Key
    bearer: http bearer — "Machine Library API key or OAuth 2.1 access token"
  audience_binding: Tokens are audience-bound to the requested MCP host (privacy policy section 4).
  flows:
    authorizationCode:
      authorizationUrl: https://api.spacefrontiers.org/v2/oauth/authorize
      client_auth: none (public clients; token_endpoint_auth_methods_supported [none])
      pkce: S256 required
      refreshUrl: https://api.spacefrontiers.org/v2/oauth/token
      registrationUrl: https://api.spacefrontiers.org/v2/oauth/register
      resource_indicator: Set the OAuth resource to https://mcp.machinelibrary.ai (auth.md section 7)
      revocationUrl: https://api.spacefrontiers.org/v2/oauth/revoke
      scopes:
        search: Search the corpus and retrieve research documents using the user's account credits.
      tokenUrl: https://api.spacefrontiers.org/v2/oauth/token
    service_auth (agent claim flow):
      constraints: Anonymous registration and external identity assertions are not accepted; the email is a login hint, not proof of identity.
      description: For agents that cannot receive a browser callback. POST https://api.spacefrontiers.org/v2/agent/identity {"type":"service_auth","login_hint":"<user email>"} returns a registration_id, a secret claim_token and a claim {user_code (6 digits), verification_uri, expires_in 900, interval 5}. The user opens the verification URI, signs in with the matching verified email, confirms the code and approves; the agent polls the token endpoint with grant_type=urn:workos:agent-auth:grant-type:claim&claim_token=... honouring authorization_pending / slow_down / access_denied / expired_token. Approval yields a one-hour access_token plus a service-signed identity_assertion; renew with grant_type=urn:ietf:params:oauth:grant-type:jwt-bearer&assertion=...
      endpoints:
        claim: https://api.spacefrontiers.org/v2/agent/identity/claim
        claim_complete: https://api.spacefrontiers.org/v2/agent/identity/claim/complete (browser-only; agents must not call it)
        identity: https://api.spacefrontiers.org/v2/agent/identity (also served on api.machinelibrary.ai)
  issuer: https://api.spacefrontiers.org
  metadata: https://api.spacefrontiers.org/.well-known/oauth-authorization-server
  name: oauth2
  protected_resource_metadata:
  - https://mcp.machinelibrary.ai/.well-known/oauth-protected-resource
  - https://machinelibrary.ai/.well-known/oauth-protected-resource
  token_lifetimes:
    access_token: 3600 seconds
    authorization_code: deleted on exchange or after 60 seconds
    refresh_token: 30 days, rotating; reuse of a rotated token revokes the chain
  type: oauth2
slug: machinelibrary-ai-authentication
source_filename: machinelibrary-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/machinelibrary-ai-openapi.yml, openapi/machinelibrary-ai-recognition-openapi.yml (securitySchemes) upgraded with https://api.machinelibrary.ai/auth.md, the RFC 8414 / RFC 9728 metadata under well-known/, https://machinelibrary.ai/privacy (token lifetimes) and the MCP repo README/smithery.yaml (key prefix)\ndocs: https://api.machinelibrary.ai/auth.md\nkeys_page: https://machinelibrary.ai/keys\nsummary:\n  types: [apiKey, http, oauth2]\n  api_key_in: [header]\n  one_credential_three_surfaces: The same API key authenticates the REST API (X-Api-Key or Bearer), the MCP server (Authorization Bearer) and the A2A agent (bearer or X-Api-Key security schemes in the card).\n  sign_in_methods: Google, GitHub, or email (press page); the /keys page 302s to /auth/signin for anonymous visitors.\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Machine Library API key from https://machinelibrary.ai/keys.\n\
  \  key_prefix: sf_live_ (example shape in the MCP README and smithery.yaml exampleConfig)\n  expiry: Long-lived; does not expire automatically, revocable from account settings (privacy policy section 4).\n  sources: [openapi/machinelibrary-ai-openapi.yml, openapi/machinelibrary-ai-recognition-openapi.yml]\n- name: bearer_auth\n  type: http\n  scheme: bearer\n  bearerFormat: API key or OAuth 2.0 access token\n  description: Send the same API key, or an OAuth 2.0 access token, as a Bearer token.\n  sources: [openapi/machinelibrary-ai-openapi.yml, openapi/machinelibrary-ai-recognition-openapi.yml]\n- name: oauth2\n  type: oauth2\n  issuer: https://api.spacefrontiers.org\n  metadata: https://api.spacefrontiers.org/.well-known/oauth-authorization-server\n  protected_resource_metadata:\n  - https://mcp.machinelibrary.ai/.well-known/oauth-protected-resource\n  - https://machinelibrary.ai/.well-known/oauth-protected-resource\n  flows:\n    authorizationCode:\n      authorizationUrl: https://api.spacefrontiers.org/v2/oauth/authorize\n\
  \      tokenUrl: https://api.spacefrontiers.org/v2/oauth/token\n      refreshUrl: https://api.spacefrontiers.org/v2/oauth/token\n      revocationUrl: https://api.spacefrontiers.org/v2/oauth/revoke\n      registrationUrl: https://api.spacefrontiers.org/v2/oauth/register\n      scopes:\n        search: Search the corpus and retrieve research documents using the user's account credits.\n      pkce: S256 required\n      client_auth: none (public clients; token_endpoint_auth_methods_supported [none])\n      resource_indicator: Set the OAuth resource to https://mcp.machinelibrary.ai (auth.md section 7)\n    service_auth (agent claim flow):\n      description: >-\n        For agents that cannot receive a browser callback. POST https://api.spacefrontiers.org/v2/agent/identity\n        {\"type\":\"service_auth\",\"login_hint\":\"<user email>\"} returns a registration_id, a secret claim_token and a\n        claim {user_code (6 digits), verification_uri, expires_in 900, interval 5}. The user opens\
  \ the verification\n        URI, signs in with the matching verified email, confirms the code and approves; the agent polls the token\n        endpoint with grant_type=urn:workos:agent-auth:grant-type:claim&claim_token=... honouring\n        authorization_pending / slow_down / access_denied / expired_token. Approval yields a one-hour access_token\n        plus a service-signed identity_assertion; renew with grant_type=urn:ietf:params:oauth:grant-type:jwt-bearer&assertion=...\n      endpoints:\n        identity: https://api.spacefrontiers.org/v2/agent/identity (also served on api.machinelibrary.ai)\n        claim: https://api.spacefrontiers.org/v2/agent/identity/claim\n        claim_complete: https://api.spacefrontiers.org/v2/agent/identity/claim/complete (browser-only; agents must not call it)\n      constraints: Anonymous registration and external identity assertions are not accepted; the email is a login hint, not proof of identity.\n  token_lifetimes:\n    access_token: 3600 seconds\n\
  \    refresh_token: 30 days, rotating; reuse of a rotated token revokes the chain\n    authorization_code: deleted on exchange or after 60 seconds\n  audience_binding: Tokens are audience-bound to the requested MCP host (privacy policy section 4).\n  a2a_card_schemes:\n    bearer: http bearer — \"Machine Library API key or OAuth 2.1 access token\"\n    apiKey: header X-Api-Key\noperation_security:\n  default: Every REST operation lists api_key OR bearer_auth (the Recognition operations inherit the same two schemes in the standalone spec); no operation is anonymous except GET /v1/pricing, which answered 200 unauthenticated on 2026-09-19.\n  unauthenticated_observations:\n  - {url: 'POST https://api.machinelibrary.ai/v2/search/', status: 401, body: '{\"detail\":\"Unauthorized\",\"status\":\"error\"}'}\n  - {url: 'POST https://mcp.machinelibrary.ai/ tools/list', status: 401, www_authenticate: 'Bearer resource_metadata=\"https://mcp.machinelibrary.ai/.well-known/oauth-protected-resource\"\
  '}\n  - {url: 'POST https://machinelibrary.ai/a2a message/send', status: 200, note: answered with an agent message describing how to authenticate}\n  - {url: 'GET https://api.machinelibrary.ai/v1/pricing', status: 200}\nsafety_rules_from_provider:\n- Never ask a user to share a password, session cookie, API key, authorization code, access token, refresh token, claim token, or identity assertion in chat. (auth.md)\n- Store claim_token as a secret; show the user only the verification_uri and user_code together; do not email the code. (auth.md)\n- Send the access token only to the configured MCP resource. (auth.md)\n- On a 401, discard the credential, re-fetch both discovery documents, and restart registration if necessary. (auth.md)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/machinelibrary-ai/refs/heads/main/authentication/machinelibrary-ai-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Research
- Scholarly Search
- Full-Text Search
- Retrieval
- RAG
- Patents
- Documents
- OCR
- Document Recognition
- MCP
- A2A
- Agent-Native
- AI Agents
- Data
- Search
---
