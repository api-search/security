---
anonymous_access: true
api_key_in: []
api_specs:
- filename: yuens-me-openapi.yml
  format: yaml
  label: Resume Agent API
  slug: resume-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yuens-me/refs/heads/main/openapi/yuens-me-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Yuens Me Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sunny Yuen declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Sunny Yuen
provider_slug: yuens-me
scheme_count: 4
schemes:
- applies_to: all public REST operations and the public MCP server
  evidence: Every public path returned 200 without an Authorization header; the card declares securitySchemes {} and security [{}].
  id: anonymous
  type: none
- applies_to:
  - POST /resume (tailored-resume generator; enforced when AUTH_MODE=key)
  - site-wide rate-limit bypass
  audience: profile owner
  evidence: GET /resume and GET /profile returned 401 {"error":"Unauthorized"} with no WWW-Authenticate header on 2026-09-19.
  id: ownerBearerKey
  scheme: bearer
  type: http
- applies_to:
  - private MCP server https://agent.yuens.me/mcp (direct API / Claude Desktop via the mcp-remote bridge)
  - site-wide rate-limit bypass
  audience: profile owner
  evidence: README security model; CORS allow-headers on /public-mcp and /mcp list x-brain-key.
  id: brainKey
  in: header
  name: x-brain-key
  type: apiKey
- applies_to:
  - private MCP server https://agent.yuens.me/mcp (rate-limit bypass on /mcp only)
  audience: profile owner's connector clients
  bearer_methods:
  - header
  client_onboarding: The client id and secret are the operator's own OAUTH_CLIENT_ID / OAUTH_CLIENT_SECRET environment variables; there is no registration endpoint (GET /register 404) and no developer sign-up. Third parties cannot obtain an OAuth client, by design.
  dynamic_client_registration: false
  evidence: /.well-known/oauth-authorization-server 200 (issuer, endpoints, grants, S256, client_secret_post); /.well-known/oauth-protected-resource 200; GET /authorize 400 (parameter validation), GET /token 404 (POST-only). CHANGELOG 2026-09-16 records client_secret becoming mandatory on the authorization_code and refresh_token grants.
  flows:
    authorizationCode:
      authorizationUrl: https://agent.yuens.me/authorize
      pkce: S256 required
      scopes: {}
      tokenUrl: https://agent.yuens.me/token
    clientCredentials:
      scopes: {}
      tokenUrl: https://agent.yuens.me/token
    refreshToken:
      tokenUrl: https://agent.yuens.me/token
  id: oauth2
  metadata:
    authorization_server: well-known/yuens-me-oauth-authorization-server.json
    protected_resource: well-known/yuens-me-oauth-protected-resource.json
  resource: https://agent.yuens.me
  response_types:
  - code
  scopes_published: false
  token_endpoint_auth_methods:
  - client_secret_post
  type: oauth2
slug: yuens-me-authentication
source_filename: yuens-me-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: >-\n  https://github.com/yuens1002/resume-agent#security-model, the live RFC 8414 / RFC 9728 documents at\n  https://agent.yuens.me/.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource,\n  and anonymous probes of every public operation on 2026-09-19. openapi/yuens-me-openapi.yml declares no\n  securitySchemes and no security requirement, which is accurate for the public surface, so the derive\n  script produced nothing and this profile is docs-sourced.\ndocs: https://github.com/yuens1002/resume-agent#security-model\nsummary: >-\n  The third-party surface is anonymous: all six REST operations, the OpenAPI document, the agent card and the\n  public MCP server answered 200 with no credential. Credentials exist only for the profile owner — a Bearer\n  API key on POST /resume, an x-brain-key header or an OAuth 2.0 access token on the private /mcp server —\n  and they double as rate-limit bypass tokens.\
  \ The OAuth authorization server on agent.yuens.me is real\n  (authorization code + PKCE, client credentials, refresh token, client_secret_post on every grant) but has\n  no registration endpoint and publishes no scopes: it exists so the owner's own claude.ai connector can\n  authenticate, not as a developer program.\npublic_surface:\n  scheme: none\n  operations: [queryProfile, matchJob, getProfile, getAvailability, listProjects, listObservations]\n  mcp_endpoint: https://agent.yuens.me/public-mcp\n  verified: '2026-09-19'\n  rate_limit: 30 requests per minute per IP (rate-limits/yuens-me-rate-limits.yml)\nschemes:\n  - id: anonymous\n    type: none\n    applies_to: all public REST operations and the public MCP server\n    evidence: Every public path returned 200 without an Authorization header; the card declares securitySchemes {} and security [{}].\n  - id: ownerBearerKey\n    type: http\n    scheme: bearer\n    audience: profile owner\n    applies_to:\n      - POST /resume (tailored-resume\
  \ generator; enforced when AUTH_MODE=key)\n      - site-wide rate-limit bypass\n    evidence: GET /resume and GET /profile returned 401 {\"error\":\"Unauthorized\"} with no WWW-Authenticate header on 2026-09-19.\n  - id: brainKey\n    type: apiKey\n    in: header\n    name: x-brain-key\n    audience: profile owner\n    applies_to:\n      - private MCP server https://agent.yuens.me/mcp (direct API / Claude Desktop via the mcp-remote bridge)\n      - site-wide rate-limit bypass\n    evidence: README security model; CORS allow-headers on /public-mcp and /mcp list x-brain-key.\n  - id: oauth2\n    type: oauth2\n    audience: profile owner's connector clients\n    applies_to:\n      - private MCP server https://agent.yuens.me/mcp (rate-limit bypass on /mcp only)\n    flows:\n      authorizationCode:\n        authorizationUrl: https://agent.yuens.me/authorize\n        tokenUrl: https://agent.yuens.me/token\n        pkce: S256 required\n        scopes: {}\n      clientCredentials:\n        tokenUrl:\
  \ https://agent.yuens.me/token\n        scopes: {}\n      refreshToken:\n        tokenUrl: https://agent.yuens.me/token\n    token_endpoint_auth_methods: [client_secret_post]\n    response_types: [code]\n    resource: https://agent.yuens.me\n    bearer_methods: [header]\n    metadata:\n      authorization_server: well-known/yuens-me-oauth-authorization-server.json\n      protected_resource: well-known/yuens-me-oauth-protected-resource.json\n    dynamic_client_registration: false\n    scopes_published: false\n    client_onboarding: >-\n      The client id and secret are the operator's own OAUTH_CLIENT_ID / OAUTH_CLIENT_SECRET environment\n      variables; there is no registration endpoint (GET /register 404) and no developer sign-up. Third\n      parties cannot obtain an OAuth client, by design.\n    evidence: >-\n      /.well-known/oauth-authorization-server 200 (issuer, endpoints, grants, S256, client_secret_post);\n      /.well-known/oauth-protected-resource 200; GET /authorize 400 (parameter\
  \ validation), GET /token 404\n      (POST-only). CHANGELOG 2026-09-16 records client_secret becoming mandatory on the authorization_code\n      and refresh_token grants.\nidentity:\n  scheme: OEP Phase 1 domain verification\n  public_key: https://agent.yuens.me/.well-known/oep-public-key.json (Ed25519)\n  dns_record: _oep.yuens.me TXT \"v=oep1; alg=ed25519; fp=bZCBY6x_RnGLyQgnCY0lN7CvpiBZMvRUBo68oeisPYc\"\n  card_field: provider.identity.fingerprint\n  verified: '2026-09-19'\n  note: 'Proves the domain owner operates the agent; it does not authenticate callers and signs nothing yet (README: no response or card signing in Phase 1).'\nmcp_auth_summary:\n  public-mcp: none\n  mcp: oauth2 or x-brain-key\nnotes:\n  - Bearer credentials are also the rate-limit bypass, so a third party must not send one it was not issued; the honest posture for agents is anonymous calls under the 30 req/min ceiling.\n  - No API-key issuance, no scopes, no OpenID Connect discovery (openid-configuration 404).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yuens-me/refs/heads/main/authentication/yuens-me-authentication.yml
summary_line: 4 schemes
tags:
- Company
- AI Agents
- A2A
- MCP
- Resume
- Hiring
- Recruiting
- Professional Profile
- Job Matching
- Open Source
---
