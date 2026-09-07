---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Elva Authentication
name_suffix: Authentication
oauth_flows: []
overview: Elva declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Elva
provider_slug: elva
scheme_count: 2
schemes:
- detail: GET /api/review/checks and POST /api/review are open to everyone, no key.
  name: none
  surface: Spec Scoring API (api.getelva.ai)
  type: none
- detail: PKCE S256 required; dynamic client registration at https://app.getelva.ai/oauth/register; token endpoint auth client_secret_post or none. No scopes_supported published in the metadata.
  flows:
    authorizationCode:
      authorizationUrl: https://app.getelva.ai/oauth/authorize
      tokenUrl: https://app.getelva.ai/oauth/token
  name: oauth2
  surface: Elva platform MCP (app.getelva.ai/mcp)
  type: oauth2
slug: elva-authentication
source_filename: elva-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: https://docs.getelva.ai/quality-and-scoring/score-a-spec-via-api\ndocs: https://docs.getelva.ai/agent-ready-with-mcp/mcp-authentication-and-oauth\nnote: >-\n  Two distinct surfaces. (1) The public Spec Scoring API at api.getelva.ai is\n  deliberately unauthenticated — \"no account and no key\" — for GET /api/review/checks\n  and POST /api/review; everything else in Elva's API (repos, catalog, collections,\n  MCP, chat, testing) sits behind authentication inside the app. (2) The platform's\n  own MCP resource at app.getelva.ai/mcp is OAuth 2.0-protected, discovered via\n  RFC 8414 + RFC 9728 metadata (probed 2026-09-07): authorization_code + PKCE S256,\n  dynamic client registration. Separately, Elva's hosted-MCP runtime RELAYS customer\n  upstream auth (no_auth, api_key, bearer_token, jwt, basic_auth, oauth_2_0\n  client-credentials/password, openid_connect) — a stateless in-memory token relay,\n  documented for customer deployments,\
  \ not an auth scheme of Elva's own API.\nschemes:\n  - name: none\n    type: none\n    surface: Spec Scoring API (api.getelva.ai)\n    detail: GET /api/review/checks and POST /api/review are open to everyone, no key.\n  - name: oauth2\n    type: oauth2\n    surface: Elva platform MCP (app.getelva.ai/mcp)\n    flows:\n      authorizationCode:\n        authorizationUrl: https://app.getelva.ai/oauth/authorize\n        tokenUrl: https://app.getelva.ai/oauth/token\n    detail: >-\n      PKCE S256 required; dynamic client registration at\n      https://app.getelva.ai/oauth/register; token endpoint auth\n      client_secret_post or none. No scopes_supported published in the metadata.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elva/refs/heads/main/authentication/elva-authentication.yml
summary_line: 2 schemes
tags:
- API Management
- MCP Server
- MCP Logs
- MCP Insights
- API Client
- API Contract
- API Governance
- API Discovery
- OpenAPI
- API Testing
- Developer Tools
- AI Agent Infrastructure
---
