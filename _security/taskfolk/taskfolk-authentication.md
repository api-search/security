---
api_key_in:
- header
api_specs:
- filename: taskfolk-product-api-openapi.yml
  format: yaml
  label: Taskfolk API
  slug: taskfolk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taskfolk/refs/heads/main/openapi/taskfolk-product-api-openapi.yml
- filename: taskfolk-agent-commerce-openapi.yml
  format: yaml
  label: Taskfolk Agent Commerce API
  slug: taskfolk-agent-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taskfolk/refs/heads/main/openapi/taskfolk-agent-commerce-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Taskfolk Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Taskfolk secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Taskfolk
provider_slug: taskfolk
scheme_count: 3
schemes:
- bearerFormat: API key
  controls:
  - per-key adjustable rate limit
  - per-key Usage tab
  - per-key Audit tab
  - anomaly detection email
  - revocation email
  description: Workspace API key. Each key is bound to exactly one workspace and carries a set of scopes. Shown in full exactly once at creation. A key acts as the user who created it, so an agent's writes are attributed to that identity; the provider recommends one key per agent.
  in: header
  key_prefix: tfk_live_
  minted_at: Workspace → Developer → Keys (and https://taskfolk.ai/me for personal access tokens)
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/taskfolk-product-api-openapi.yml
  - https://taskfolk.ai/auth.md
  type: http
- access_token_ttl: 1 hour
  declared_in_openapi: false
  detail: scopes/taskfolk-scopes.yml
  flows:
  - authorizationUrl: https://taskfolk.ai/api/oauth/authorize
    flow: authorizationCode
    pkce: S256 required on every code exchange
    refreshUrl: https://taskfolk.ai/api/oauth/token
    scopes_count: 47
    tokenUrl: https://taskfolk.ai/api/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://taskfolk.ai
  name: oauth2
  refresh_token_ttl: 30 days
  registration_endpoint: https://taskfolk.ai/api/oauth/register
  revocation_endpoint: https://taskfolk.ai/api/oauth/revoke
  sources:
  - https://taskfolk.ai/.well-known/oauth-authorization-server
  - https://taskfolk.ai/auth.md
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  type: oauth2
- description: Long-lived human-minted token at https://taskfolk.ai/me, handed to an agent. Inherits the creator's role ceiling and chosen scopes.
  name: personal-access-token
  scheme: bearer
  sources:
  - https://taskfolk.ai/auth.md
  - https://taskfolk.ai/.well-known/agent-card.json
  type: http
slug: taskfolk-authentication
source_filename: taskfolk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-20'\nmethod: searched\nsource: openapi/taskfolk-product-api-openapi.yml\ndocs: https://taskfolk.ai/auth.md\ndiscovery:\n  authorization_server: https://taskfolk.ai/.well-known/oauth-authorization-server\n  protected_resource: https://taskfolk.ai/.well-known/oauth-protected-resource\n  agent_card: https://taskfolk.ai/.well-known/agent-card.json\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  pkce: required (S256)\n  dynamic_client_registration: true\nnote: >-\n  The derived pass found ONE scheme (bearerAuth) because that is all the OpenAPI declares.\n  The docs pass adds the OAuth 2.0 authorization server, which is real and fully described in\n  RFC 8414 / RFC 9728 discovery documents but is absent from the contract's securitySchemes.\n  Both credential types resolve to the same `Authorization: Bearer` header on the wire, and\n  the same token works on REST and MCP.\nschemes:\n \
  \ - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: API key\n    in: header\n    key_prefix: tfk_live_\n    description: >-\n      Workspace API key. Each key is bound to exactly one workspace and carries a set of\n      scopes. Shown in full exactly once at creation. A key acts as the user who created it,\n      so an agent's writes are attributed to that identity; the provider recommends one key\n      per agent.\n    minted_at: Workspace → Developer → Keys (and https://taskfolk.ai/me for personal access tokens)\n    controls: [per-key adjustable rate limit, per-key Usage tab, per-key Audit tab, anomaly detection email, revocation email]\n    sources: [openapi/taskfolk-product-api-openapi.yml, https://taskfolk.ai/auth.md]\n  - name: oauth2\n    type: oauth2\n    declared_in_openapi: false\n    issuer: https://taskfolk.ai\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://taskfolk.ai/api/oauth/authorize\n        tokenUrl: https://taskfolk.ai/api/oauth/token\n\
  \        refreshUrl: https://taskfolk.ai/api/oauth/token\n        scopes_count: 47\n        pkce: S256 required on every code exchange\n    revocation_endpoint: https://taskfolk.ai/api/oauth/revoke\n    registration_endpoint: https://taskfolk.ai/api/oauth/register\n    grant_types: [authorization_code, refresh_token]\n    token_endpoint_auth_methods: [none, client_secret_post]\n    access_token_ttl: 1 hour\n    refresh_token_ttl: 30 days\n    sources: [https://taskfolk.ai/.well-known/oauth-authorization-server, https://taskfolk.ai/auth.md]\n    detail: scopes/taskfolk-scopes.yml\n  - name: personal-access-token\n    type: http\n    scheme: bearer\n    description: >-\n      Long-lived human-minted token at https://taskfolk.ai/me, handed to an agent. Inherits\n      the creator's role ceiling and chosen scopes.\n    sources: [https://taskfolk.ai/auth.md, https://taskfolk.ai/.well-known/agent-card.json]\nagent_onboarding:\n  anonymous_registration: true\n  flow: >-\n    1) discover the AS\
  \ metadata, 2) POST an unauthenticated RFC 7591 client registration\n    naming the target workspace slug, 3) send the user through the claim ceremony\n    (authorization_code + PKCE S256) where they sign in passwordlessly and approve the\n    scopes, 4) exchange the code, 5) call REST or MCP with the same Bearer token,\n    6) refresh, 7) revoke (RFC 7009).\n  human_consent_required: true\n  revocable_by_user: Workspace Developer dashboard; revoked credentials fail with an opaque 401.\n  machine_readable_at: agent_auth block inside the RFC 8414 metadata\n  docs: https://taskfolk.ai/auth.md\nchallenge_observed:\n  url: https://taskfolk.ai/api/mcp/v1\n  http_status: 401\n  www_authenticate: 'Bearer realm=\"taskfolk-product\", resource_metadata=\"https://taskfolk.ai/.well-known/oauth-protected-resource\"'\n  note: RFC 9728-compliant challenge — the 401 points a client straight at the protected-resource metadata.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taskfolk/refs/heads/main/authentication/taskfolk-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Project Management
- Issue Tracking
- Task Management
- Productivity
- Collaboration
- MCP
- AI Agents
- agent-native
- Agentic Commerce
- A2A
- REST API
- OpenAPI
- Webhook
- Authentication
- Agile
- Sprints
- OKR
- Developer Tools
---
