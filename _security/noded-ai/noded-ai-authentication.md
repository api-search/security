---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Noded Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Noded AI declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Noded AI
provider_slug: noded-ai
scheme_count: 3
schemes:
- audience: provisioned per customer (the Noded API audience)
  client_id: provisioned per customer (SPA client)
  default: true
  flow: authorization_code
  issuer: https://login.getnoded.ai/
  name: oidc
  permissions: calls are automatically scoped to the signed-in user's tenant and permissions; the API enforces them server-side
  pkce: true
  provider: Auth0
  recommended_for: browser / SPA
  redirect_uri: defaults to window.location.origin
  refresh: silent refresh via offline_access
  response_type: code
  scope_default: openid profile email offline_access
  secrets_in_browser: false
  token_placement: 'Authorization: Bearer <access_token>'
  type: openIdConnect
- name: token
  note: caller supplies getToken(); the SDK does not manage the lifecycle
  recommended_for: server-rendered apps that already ran their own OIDC flow
  scheme: bearer
  token_placement: 'Authorization: Bearer <access_token>'
  type: http
- caveat: The credential is transported as a colon-delimited composite inside a Bearer token rather than a standard bearer credential; it is not an OAuth 2.0 access token.
  name: apiKey
  recommended_for: server only
  requires:
  - apiKey — a Noded service or personal access token
  - actAs — the tenant email the key acts as
  scheme: bearer
  token_placement: 'Authorization: Bearer apiKey:<apiKey>:<actAs>'
  type: http
  warning: Provider states explicitly this must NEVER be shipped to a browser. Noded's own README notes a first-class Personal Access Token flow is still "on the roadmap", so this composite Bearer string is the current server path.
slug: noded-ai-authentication
source_filename: noded-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://www.getnoded.ai/developers\ndocs: https://www.getnoded.ai/developers\nsupporting_source: >-\n  https://www.getnoded.ai/developers/AGENTS.md and npm @bigfootai/noded-sdk@0.1.2\n  (dist/index.d.ts AuthConfig, dist/index.js authorization())\nnote: >-\n  Noded has no self-serve API credential flow. The developer page states plainly that the\n  issuer, client ID and API audience are \"provided by Noded\" after you request access and send\n  them your app origins — so obtaining credentials is a human handoff via getnoded.ai/contact-us,\n  not a console. The mechanism itself (Auth0 OIDC authorization-code + PKCE, silent refresh) is\n  fully documented in public.\nsummary: >-\n  Three auth modes over one Bearer-token GraphQL endpoint. Browser apps use OIDC against a\n  Noded-hosted Auth0 tenant; servers may use an API key; callers with their own OIDC flow may\n  supply a token directly.\nschemes:\n  - name: oidc\n    type:\
  \ openIdConnect\n    default: true\n    recommended_for: browser / SPA\n    issuer: https://login.getnoded.ai/\n    provider: Auth0\n    flow: authorization_code\n    pkce: true\n    response_type: code\n    audience: provisioned per customer (the Noded API audience)\n    client_id: provisioned per customer (SPA client)\n    redirect_uri: defaults to window.location.origin\n    scope_default: openid profile email offline_access\n    refresh: silent refresh via offline_access\n    token_placement: 'Authorization: Bearer <access_token>'\n    secrets_in_browser: false\n    permissions: >-\n      calls are automatically scoped to the signed-in user's tenant and permissions; the API\n      enforces them server-side\n  - name: token\n    type: http\n    scheme: bearer\n    recommended_for: server-rendered apps that already ran their own OIDC flow\n    token_placement: 'Authorization: Bearer <access_token>'\n    note: caller supplies getToken(); the SDK does not manage the lifecycle\n  - name:\
  \ apiKey\n    type: http\n    scheme: bearer\n    recommended_for: server only\n    token_placement: 'Authorization: Bearer apiKey:<apiKey>:<actAs>'\n    requires:\n      - apiKey — a Noded service or personal access token\n      - actAs — the tenant email the key acts as\n    warning: >-\n      Provider states explicitly this must NEVER be shipped to a browser. Noded's own README\n      notes a first-class Personal Access Token flow is still \"on the roadmap\", so this composite\n      Bearer string is the current server path.\n    caveat: >-\n      The credential is transported as a colon-delimited composite inside a Bearer token rather\n      than a standard bearer credential; it is not an OAuth 2.0 access token.\nmutual_tls: false\ncredential_self_serve: false\ncredential_request_url: https://www.getnoded.ai/contact-us\nembedding_pattern:\n  - name: server proxy\n    description: >-\n      When viewers are not Noded users, run a proxy that holds the credential and point the SDK\n \
  \     at it via the endpoint option; the browser never sees the token.\nerror_on_auth_failure:\n  kind: auth\n  message: Not authorized — sign in again (noded.connect())\n  remediation: re-run noded.connect()\nscheme_count: 3\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noded-ai/refs/heads/main/authentication/noded-ai-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Ai Ml
- Customer Success
- Customer Data
- Churn
- Retention
- Revenue Operations
- Software-as-a-Service
- AI Agents
- GraphQL
- MCP
- Agent Native
- Customer Context Graph
---
