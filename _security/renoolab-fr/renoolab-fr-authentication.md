---
anonymous_access: true
api_key_in: []
auth_types:
- none
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Renoolab Fr Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: RenooLab secures its APIs with none and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: RenooLab
provider_slug: renoolab-fr
scheme_count: 2
schemes:
- applies_to:
  - rechercher_artisans
  - rechercher_chantier
  - A2A https://a2a.renoolab.fr/a2a
  - MCP initialize / tools/list / resources/list
  description: Anonymous access; the server applies per-actor quotas (see rate-limits/renoolab-fr-rate-limits.yml) using pseudonymous actor ids and an HMAC of the IP (privacy policy §2).
  name: noauth
  sources:
  - mcp/renoolab-fr-mcp-tools-list.json
  type: none
- account_required: false
  applies_to:
  - contacter_artisan
  - creer_profil_artisan
  authorization_server_metadata: well-known/renoolab-fr-oauth-authorization-server.json
  bearer_methods:
  - header
  consent: all four tools in one grant (docs); the two read tools do not actually require the token
  consent_cookies: 'two strictly-necessary HttpOnly cookies during consent: a 10-minute anti-CSRF token and a 12-month pseudonymous browser id used to manage and revoke OAuth grants (privacy policy §7)'
  dynamic_client_registration: https://mcp.renoolab.fr/register
  flows:
  - authorizationUrl: https://mcp.renoolab.fr/authorize
    flow: authorizationCode
    pkce: S256
    refreshUrl: https://mcp.renoolab.fr/token
    scopes: {}
    tokenUrl: https://mcp.renoolab.fr/token
  issuer: https://mcp.renoolab.fr
  name: RenooLabOAuth
  protected_resource_metadata: well-known/renoolab-fr-oauth-protected-resource.json
  revocation_endpoint: https://mcp.renoolab.fr/token
  sources:
  - mcp/renoolab-fr-mcp-tools-list.json
  - well-known/renoolab-fr-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  token_lifetimes:
    access_token: 1 hour
    consent_session: 10 minutes
    dynamic_client: 90 days
    refresh_token: 30 days
    source: https://renoolab.fr/privacy/ §5
  type: oauth2
slug: renoolab-fr-authentication
source_filename: renoolab-fr-authentication.yml
source_heading: Authentication Profile
source_url: https://mcp.renoolab.fr/mcp (tools/list _meta.securitySchemes, 2026-09-19)
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://mcp.renoolab.fr/mcp\ndocs:\n- https://renoolab.fr/mcp/\n- https://github.com/mehdimicra/renoolab-mcp/blob/main/llms-install.md\n- https://renoolab.fr/privacy/\nsources:\n- https://mcp.renoolab.fr/mcp (tools/list _meta.securitySchemes, 2026-09-19)\n- https://mcp.renoolab.fr/.well-known/oauth-authorization-server\n- https://mcp.renoolab.fr/.well-known/oauth-protected-resource\n- https://renoolab.fr/.well-known/agent-card.json\nsummary:\n  types: [none, oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  bearer: true\n  headline: >-\n    Two tiers on one MCP endpoint. Reads (rechercher_artisans, rechercher_chantier) are anonymous - tools/list\n    and the tools themselves declare {type: noauth} and the endpoint answered initialize/tools/list with no\n    credential. Writes (contacter_artisan, creer_profil_artisan) require an OAuth 2.1 bearer token from the\n    provider's own authorization server at https://mcp.renoolab.fr:\
  \ authorization code + PKCE S256, dynamic\n    client registration (RFC 7591), refresh tokens, revocation, token endpoint auth incl. `none` for public\n    clients, bearer in the Authorization header (RFC 9728 bearer_methods_supported). No RenooLab account is\n    required to complete the consent, no API keys exist, and the install guide instructs clients to add NO\n    headers, keys, client_id or secret to the configuration. The A2A agent is read-only and anonymous (no\n    securitySchemes in the card). The WebMCP in-page tools run in the user's browser session against the\n    site's own Worker; the two write tools there require a visible human confirmation in the page.\nschemes:\n- name: noauth\n  type: none\n  applies_to: [rechercher_artisans, rechercher_chantier, 'A2A https://a2a.renoolab.fr/a2a', 'MCP initialize / tools/list / resources/list']\n  description: Anonymous access; the server applies per-actor quotas (see rate-limits/renoolab-fr-rate-limits.yml) using pseudonymous actor\
  \ ids and an HMAC of the IP (privacy policy §2).\n  sources: [mcp/renoolab-fr-mcp-tools-list.json]\n- name: RenooLabOAuth\n  type: oauth2\n  applies_to: [contacter_artisan, creer_profil_artisan]\n  issuer: https://mcp.renoolab.fr\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.renoolab.fr/authorize\n    tokenUrl: https://mcp.renoolab.fr/token\n    refreshUrl: https://mcp.renoolab.fr/token\n    pkce: S256\n    scopes: {}\n  dynamic_client_registration: https://mcp.renoolab.fr/register\n  revocation_endpoint: https://mcp.renoolab.fr/token\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\n  bearer_methods: [header]\n  protected_resource_metadata: well-known/renoolab-fr-oauth-protected-resource.json\n  authorization_server_metadata: well-known/renoolab-fr-oauth-authorization-server.json\n  account_required: false\n  consent: all four tools in one grant (docs); the two read tools do not actually require the token\n  token_lifetimes: {access_token:\
  \ 1 hour, refresh_token: 30 days, dynamic_client: 90 days, consent_session: 10 minutes, source: 'https://renoolab.fr/privacy/ §5'}\n  consent_cookies: 'two strictly-necessary HttpOnly cookies during consent: a 10-minute anti-CSRF token and a 12-month pseudonymous browser id used to manage and revoke OAuth grants (privacy policy §7)'\n  sources: [mcp/renoolab-fr-mcp-tools-list.json, well-known/renoolab-fr-oauth-authorization-server.json]\nobserved:\n- {request: 'POST /mcp tools/list without credentials', result: 200 - full tool list}\n- {request: 'GET /mcp', result: 406 application/json (Accept negotiation, not auth)}\n- {request: 'GET /register', result: 405}\n- {request: 'GET /authorize', result: 400}\n- {request: 'GET /mcp/index.md on the MCP host', result: 401 application/json}\nnot_used: [apiKey, http basic, openIdConnect, mutualTLS]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/renoolab-fr/refs/heads/main/authentication/renoolab-fr-authentication.yml
summary_line: none/oauth2 · 2 schemes
tags:
- Home Services
- Construction
- Building Trades
- Renovation
- Marketplace
- Local Services
- MCP
- A2A
- AI Agents
- Agent Skills
- France
---
