---
anonymous_access: false
api_key_in: []
api_specs:
- filename: chikoh-com-contest-intelligence-api-openapi.yml
  format: yaml
  label: Chikoh Contest Intelligence API
  slug: chikoh-com-contest-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chikoh-com/openapi/chikoh-com-contest-intelligence-api-openapi.yml
- filename: chikoh-com-entertainment-api-openapi.yml
  format: yaml
  label: Chikoh Entertainment API
  slug: chikoh-com-entertainment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chikoh-com/openapi/chikoh-com-entertainment-api-openapi.yml
- filename: chikoh-com-entertainment-predictions-api-openapi.yml
  format: yaml
  label: Chikoh Entertainment Predictions API
  slug: chikoh-com-entertainment-predictions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chikoh-com/openapi/chikoh-com-entertainment-predictions-api-openapi.yml
- filename: chikoh-com-market-intelligence-api-openapi.yml
  format: yaml
  label: Chikoh Market Intelligence API
  slug: chikoh-com-market-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chikoh-com/openapi/chikoh-com-market-intelligence-api-openapi.yml
- filename: chikoh-com-player-intelligence-api-openapi.yml
  format: yaml
  label: Chikoh Player Intelligence API
  slug: chikoh-com-player-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chikoh-com/openapi/chikoh-com-player-intelligence-api-openapi.yml
- filename: chikoh-com-strategic-intelligence-api-openapi.yml
  format: yaml
  label: Chikoh Strategic Intelligence API
  slug: chikoh-com-strategic-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chikoh-com/openapi/chikoh-com-strategic-intelligence-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Chikoh Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Chikoh secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Chikoh
provider_slug: chikoh-com
scheme_count: 2
schemes:
- description: Sign in with your Chikoh account. Required for Syndicate tools.
  flows:
  - authorizationUrl: https://chikoh.com/api/v1/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://chikoh.com/api/v1/oauth/token
  name: oauth2
  sources:
  - openapi/chikoh-com-openapi.yml
  type: oauth2
- description: Agent API key (chk_agent_*). Register at /api/v1/agent/register
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/chikoh-com-openapi.yml
  type: http
slug: chikoh-com-authentication
source_filename: chikoh-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://chikoh.com/developers\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://chikoh.com/api/v1/oauth/authorize\n    tokenUrl: https://chikoh.com/api/v1/oauth/token\n    scopes: 2\n  description: Sign in with your Chikoh account. Required for Syndicate tools.\n  sources:\n  - openapi/chikoh-com-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Agent API key (chk_agent_*). Register at /api/v1/agent/register\n  sources:\n  - openapi/chikoh-com-openapi.yml\ndocs: https://chikoh.com/developers\ndocumented_key_types:\n- prefix: chk_user_\n  name: Personal Key\n  text: For connecting your own Chikoh account to tools. Included with any subscription. Get it from Settings → API Keys.\n- prefix: chk_agent_\n  name: Developer Key\n  text: For building apps that\
  \ serve other users . $29+/mo with metered billing. Register at /developers/get-api-key\n- prefix: sk_live_ / sk_test_\n  name: B2B tenant keys\n  text: 'Authorization: Bearer sk_live_... Use sk_test_ during development.'\n  source: https://chikoh.com/developers/byoo-webhook\nanonymous_access: 'Free: 10 calls/hour without auth. Authenticate via OAuth for premium features.'\noauth_docs_note: 'Developers page documents Authorization URL https://chikoh.com/api/v1/oauth/authorize, Token URL https://chikoh.com/api/v1/oauth/token, Scope: read; changelog 2.3.0 states \"OAuth 2.1 + PKCE authentication for AI agent integrations\".'\n"
source_yaml_url: https://artifacts.apis.io/chikoh-com/authentication/chikoh-com-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Fantasy Sports
- Sports Analytics
- Reality TV
- Predictions
- Gaming
- AI Agents
- MCP
---
