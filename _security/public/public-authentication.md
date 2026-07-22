---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Public Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Public secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Public
provider_slug: public
scheme_count: 2
schemes:
- bearer_format: JWT
  description: 'Primary auth for the direct Trading API. A long-lived, revocable secret key is generated in account settings (https://public.com/settings/v2/api), then exchanged for a short-lived access-token JWT via POST https://api.public.com/userapiauthservice/personal/access-tokens (body: {secret, validityInMinutes}; default validity 15 min). The returned accessToken is sent as `Authorization: Bearer <token>` on gateway calls under https://api.public.com/userapigateway/trading/.'
  name: PersonalAccessToken
  scheme: bearer
  sources:
  - https://public.com/api/docs/quickstart
  type: http
- description: 'Used by the hosted MCP server (mcp.public.com) for AI-assistant connectors (Claude, ChatGPT). Authorization server: https://prod-api.154310543964.hellopublic.com/userapiauthservice/oauth2. Scopes: trading.read, trading.write, marketdata, openid (see scopes/).'
  name: OAuth2
  sources:
  - https://mcp.public.com/.well-known/oauth-protected-resource
  type: oauth2
slug: public-authentication
source_filename: public-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://public.com/api/docs/quickstart\ndocs: https://public.com/api/docs/resources/authorization/create-personal-access-token\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  bearer_format: JWT\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: PersonalAccessToken\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  description: >-\n    Primary auth for the direct Trading API. A long-lived, revocable secret key\n    is generated in account settings (https://public.com/settings/v2/api), then\n    exchanged for a short-lived access-token JWT via\n    POST https://api.public.com/userapiauthservice/personal/access-tokens\n    (body: {secret, validityInMinutes}; default validity 15 min). The returned\n    accessToken is sent as `Authorization: Bearer <token>` on gateway calls under\n    https://api.public.com/userapigateway/trading/.\n  sources: [https://public.com/api/docs/quickstart]\n- name: OAuth2\n\
  \  type: oauth2\n  description: >-\n    Used by the hosted MCP server (mcp.public.com) for AI-assistant connectors\n    (Claude, ChatGPT). Authorization server:\n    https://prod-api.154310543964.hellopublic.com/userapiauthservice/oauth2.\n    Scopes: trading.read, trading.write, marketdata, openid (see scopes/).\n  sources: [https://mcp.public.com/.well-known/oauth-protected-resource]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/public/refs/heads/main/authentication/public-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Consumer
- Investing
- Brokerage
- Trading
- Fintech
- Stocks
- Options
- Crypto
- Market Data
- Agentic
- MCP
---
