---
anonymous_access: false
api_key_in: []
api_specs:
- filename: marketintell-ai-agent-execution-api-openapi.yml
  format: yaml
  label: MarketIntell Agent Execution API
  slug: marketintell-ai-agent-execution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketintell-ai/openapi/marketintell-ai-agent-execution-api-openapi.yml
- filename: marketintell-ai-agents-api-openapi.yml
  format: yaml
  label: MarketIntell Agents API
  slug: marketintell-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketintell-ai/openapi/marketintell-ai-agents-api-openapi.yml
- filename: marketintell-ai-alpha-api-openapi.yml
  format: yaml
  label: MarketIntell Alpha API
  slug: marketintell-ai-alpha-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketintell-ai/openapi/marketintell-ai-alpha-api-openapi.yml
- filename: marketintell-ai-billing-api-openapi.yml
  format: yaml
  label: MarketIntell Billing API
  slug: marketintell-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketintell-ai/openapi/marketintell-ai-billing-api-openapi.yml
- filename: marketintell-ai-brain-api-openapi.yml
  format: yaml
  label: MarketIntell Brain API
  slug: marketintell-ai-brain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketintell-ai/openapi/marketintell-ai-brain-api-openapi.yml
- filename: marketintell-ai-brokers-api-openapi.yml
  format: yaml
  label: MarketIntell Brokers API
  slug: marketintell-ai-brokers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketintell-ai/openapi/marketintell-ai-brokers-api-openapi.yml
- filename: marketintell-ai-leaderboard-api-openapi.yml
  format: yaml
  label: MarketIntell Leaderboard API
  slug: marketintell-ai-leaderboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketintell-ai/openapi/marketintell-ai-leaderboard-api-openapi.yml
- filename: marketintell-ai-proof-api-openapi.yml
  format: yaml
  label: MarketIntell Proof API
  slug: marketintell-ai-proof-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketintell-ai/openapi/marketintell-ai-proof-api-openapi.yml
- filename: marketintell-ai-screener-api-openapi.yml
  format: yaml
  label: MarketIntell Screener API
  slug: marketintell-ai-screener-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketintell-ai/openapi/marketintell-ai-screener-api-openapi.yml
- filename: marketintell-ai-sessions-api-openapi.yml
  format: yaml
  label: MarketIntell Sessions API
  slug: marketintell-ai-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketintell-ai/openapi/marketintell-ai-sessions-api-openapi.yml
- filename: marketintell-ai-signals-api-openapi.yml
  format: yaml
  label: MarketIntell Signals API
  slug: marketintell-ai-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketintell-ai/openapi/marketintell-ai-signals-api-openapi.yml
- filename: marketintell-ai-system-api-openapi.yml
  format: yaml
  label: MarketIntell System API
  slug: marketintell-ai-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketintell-ai/openapi/marketintell-ai-system-api-openapi.yml
- filename: marketintell-ai-trades-api-openapi.yml
  format: yaml
  label: MarketIntell Trades API
  slug: marketintell-ai-trades-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketintell-ai/openapi/marketintell-ai-trades-api-openapi.yml
- filename: marketintell-ai-webhooks-api-openapi.yml
  format: yaml
  label: MarketIntell Webhooks API
  slug: marketintell-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketintell-ai/openapi/marketintell-ai-webhooks-api-openapi.yml
auth_types: []
description: 'All MarketIntell API endpoints require authentication via an API key. Keys can be passed in three ways: Authorization: Bearer <key> header (recommended), X-API-Key: <key> header, ?api_key=<key> query parameter (for SSE connections only — not recommended for general use).'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: MarketIntell Authentication
name_suffix: Authentication
oauth_flows: []
overview: MarketIntell declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MarketIntell
provider_slug: marketintell-ai
scheme_count: 1
schemes:
- evidence: 'All MarketIntell API endpoints require authentication via an API key. Keys can be passed in three ways: Authorization: Bearer <key> header (recommended)'
  header: Authorization
  location: header
  name: Authorization Bearer
  type: apiKey
slug: marketintell-ai-authentication
source_filename: marketintell-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.marketintell.ai/docs/authentication
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.marketintell.ai/docs/authentication\nsources:\n- https://docs.marketintell.ai/docs/authentication\n- https://docs.marketintell.ai/docs/web-bot-auth\n- https://docs.marketintell.ai/docs/api/auth\n- https://docs.marketintell.ai/docs/api/tokens\ndescription: 'All MarketIntell API endpoints require authentication via an API key. Keys can be passed in three ways: Authorization: Bearer <key>\n  header (recommended), X-API-Key: <key> header, ?api_key=<key> query parameter (for SSE connections only — not recommended for general use).'\nschemes:\n- type: apiKey\n  name: Authorization Bearer\n  evidence: 'All MarketIntell API endpoints require authentication via an API key. Keys can be passed in three ways: Authorization: Bearer <key>\n    header (recommended)'\n  location: header\n  header: Authorization\nnote: API keys are created via POST /v1/auth/signup (free tier, no auth\
  \ required) or POST /v1/auth/keys (requires admin scope). 2 extracted row(s)\n  were dropped because their quote was not on the page.\ndocs: https://docs.marketintell.ai/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/marketintell-ai/authentication/marketintell-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Market Intelligence
- Cryptocurrency
- Stocks
- Trading Signals
---
