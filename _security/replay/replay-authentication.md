---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Replay Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- deviceCode
overview: Replay secures its APIs with apiKey, oauth2, and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and deviceCode flow(s).
provider_name: Replay
provider_slug: replay
scheme_count: 2
schemes:
- applies_to:
  - GraphQL API
  - MCP server
  - CLI
  - Playwright/Cypress reporters
  - source-map upload
  description: 'Programmatic access to the GraphQL API (https://api.replay.io/v1/graphql) and the Replay MCP server (https://dispatch.replay.io/nut/mcp) uses a Replay API key presented as a bearer token: `Authorization: Bearer ${REPLAY_API_KEY}`. Keys are created under Settings > API Keys at https://app.replay.io/team/settings and are commonly set as the REPLAY_API_KEY env var for the CLI and test integrations.

    '
  docs: https://docs.replay.io/reference/integrations/replay-apis/graphql-api
  name: ReplayApiKey
  scheme: bearer
  type: http
- description: 'Interactive login to the Replay web app is delegated to an Auth0 tenant (webreplay.us.auth0.com). Discovery documents are served from app.replay.io and expose the authorization, token, device-authorization, userinfo, and revocation endpoints. `replayio login` uses this flow via the browser.

    '
  flows:
  - authorizationCode
  - deviceCode
  issuer: https://webreplay.us.auth0.com/
  name: Auth0OIDC
  openIdConnectUrl: https://app.replay.io/.well-known/openid-configuration
  source: well-known/replay-openid-configuration.json
  type: openIdConnect
slug: replay-authentication
source_filename: replay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.replay.io/reference/integrations/replay-apis/graphql-api\ndocs: https://docs.replay.io/reference/replay-cli/commands\nsummary:\n  types: [apiKey, oauth2, openIdConnect]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, deviceCode]\nschemes:\n  - name: ReplayApiKey\n    type: http\n    scheme: bearer\n    description: >\n      Programmatic access to the GraphQL API (https://api.replay.io/v1/graphql) and the Replay\n      MCP server (https://dispatch.replay.io/nut/mcp) uses a Replay API key presented as a bearer\n      token: `Authorization: Bearer ${REPLAY_API_KEY}`. Keys are created under Settings > API Keys\n      at https://app.replay.io/team/settings and are commonly set as the REPLAY_API_KEY env var for\n      the CLI and test integrations.\n    docs: https://docs.replay.io/reference/integrations/replay-apis/graphql-api\n    applies_to: [GraphQL API, MCP server, CLI, Playwright/Cypress reporters,\
  \ source-map upload]\n  - name: Auth0OIDC\n    type: openIdConnect\n    openIdConnectUrl: https://app.replay.io/.well-known/openid-configuration\n    issuer: https://webreplay.us.auth0.com/\n    description: >\n      Interactive login to the Replay web app is delegated to an Auth0 tenant\n      (webreplay.us.auth0.com). Discovery documents are served from app.replay.io and expose the\n      authorization, token, device-authorization, userinfo, and revocation endpoints. `replayio\n      login` uses this flow via the browser.\n    source: well-known/replay-openid-configuration.json\n    flows: [authorizationCode, deviceCode]\nnotes: >\n  No OpenAPI is published (the primary programmatic surface is GraphQL), so this profile is\n  searched from the docs and the live OIDC discovery documents rather than derived from a spec.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/replay/refs/heads/main/authentication/replay-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 2 schemes
tags:
- Company
- Debugging
- Testing
- Quality Assurance
- Developer Tools
- Time Travel Debugging
- MCP
- GraphQL
- Browser Automation
- AI
---
