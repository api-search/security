---
api_key_in:
- header
api_specs:
- filename: fundz-acquisitions-api-openapi.yml
  format: yaml
  label: Fundz Acquisitions API
  slug: fundz-acquisitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundz/refs/heads/main/openapi/fundz-acquisitions-api-openapi.yml
- filename: fundz-agreements-api-openapi.yml
  format: yaml
  label: Fundz Agreements API
  slug: fundz-agreements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundz/refs/heads/main/openapi/fundz-agreements-api-openapi.yml
- filename: fundz-crowdfundings-api-openapi.yml
  format: yaml
  label: Fundz Crowdfundings API
  slug: fundz-crowdfundings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundz/refs/heads/main/openapi/fundz-crowdfundings-api-openapi.yml
- filename: fundz-executives-api-openapi.yml
  format: yaml
  label: Fundz Executives API
  slug: fundz-executives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundz/refs/heads/main/openapi/fundz-executives-api-openapi.yml
- filename: fundz-fundings-api-openapi.yml
  format: yaml
  label: Fundz Fundings API
  slug: fundz-fundings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundz/refs/heads/main/openapi/fundz-fundings-api-openapi.yml
- filename: fundz-products-api-openapi.yml
  format: yaml
  label: Fundz Products API
  slug: fundz-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundz/refs/heads/main/openapi/fundz-products-api-openapi.yml
auth_types:
- apiKey
- http-bearer
description: Fundz runs two authenticated surfaces on one host. The core feed API takes the API key as the RAW value of the Authorization header — no `Bearer` prefix — and is paid-plans-only. The FundzWatch surface at /v1/watch/* takes a prefixed key (fundz_test_ / fundz_live_) as a Bearer token and has a free developer tier. Both are api-key models; neither publishes an OAuth authorization server, despite the core docs saying a Bearer access token is accepted for ChatGPT/agent integrations.
kind: authentication
layout: security
method: searched
name: Fundz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fundz secures its APIs with apiKey and http-bearer across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Fundz
provider_slug: fundz
scheme_count: 4
schemes:
- applied: globally via root security[] on all six operations
  bearer_prefix: false
  description: The key is the raw header value. The spec is emphatic about this — "no `Bearer` prefix" — which is worth honouring, because it is the opposite of the FundzWatch surface on the same host.
  example: 'curl -H "Authorization: YOUR_API_KEY" https://api.fundz.net/companies/onelayer'
  id: apiKey
  in: header
  name: Authorization
  source: openapi/_original/fundz-openapi.json#/components/securitySchemes/apiKey
  surface: core
  type: apiKey
- description: '"For ChatGPT and other agent integrations, the API also accepts an OAuth access token using the Bearer scheme: Authorization: Bearer <access_token>." No authorization endpoint, token endpoint, client registration or scope list is published, and /.well-known/oauth-authorization-server 404s on every host — so this is an accepted credential format rather than a documented OAuth 2.0 deployment. No scopes/ artifact was written for exactly this reason.'
  id: oauthBearer
  in: header
  in_openapi: false
  name: Authorization
  scheme: bearer
  source: https://app.fundz.net/knowledge/api-references/authentication
  surface: core
  type: http
- description: In-app browser usage is authenticated by a logged-in session cookie. Not for programmatic use.
  id: sessionCookie
  source: https://app.fundz.net/knowledge/api-references/authentication
  surface: in-app browser
  type: cookie
- base: https://api.fundz.net/v1/watch
  description: Prefixed, mode-separated keys with a Bearer scheme — a materially more modern auth posture than the core API's raw header, on the same hostname.
  environment_variable: FUNDZWATCH_API_KEY
  example: 'curl https://api.fundz.net/v1/watch/events -H "Authorization: Bearer YOUR_API_KEY"'
  id: fundzwatchBearer
  in: header
  in_openapi: false
  key_prefixes:
  - mode: test
    note: Developer-tier limits, live data.
    prefix: fundz_test_
  - mode: live
    note: Paid plans.
    prefix: fundz_live_
  name: Authorization
  scheme: bearer
  source: https://fundzwatch.ai/docs
  surface: fundzwatch
  type: http
slug: fundz-authentication
source_filename: fundz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nstatus: published\nsource: https://app.fundz.net/knowledge/api-references/authentication, https://fundzwatch.ai/docs, openapi/_original/fundz-openapi.json\ndescription: >-\n  Fundz runs two authenticated surfaces on one host. The core feed API takes the API key as the\n  RAW value of the Authorization header — no `Bearer` prefix — and is paid-plans-only. The\n  FundzWatch surface at /v1/watch/* takes a prefixed key (fundz_test_ / fundz_live_) as a Bearer\n  token and has a free developer tier. Both are api-key models; neither publishes an OAuth\n  authorization server, despite the core docs saying a Bearer access token is accepted for\n  ChatGPT/agent integrations.\nverified: '2026-08-14'\nsummary:\n  types: [apiKey, http-bearer]\n  api_key_in: [header]\n  oauth2_flows: []\n  mtls: false\n  openid_connect: false\nschemes:\n- id: apiKey\n  surface: core\n  type: apiKey\n  in: header\n  name: Authorization\n  bearer_prefix: false\n \
  \ source: openapi/_original/fundz-openapi.json#/components/securitySchemes/apiKey\n  applied: globally via root security[] on all six operations\n  example: 'curl -H \"Authorization: YOUR_API_KEY\" https://api.fundz.net/companies/onelayer'\n  description: >-\n    The key is the raw header value. The spec is emphatic about this — \"no `Bearer` prefix\" — which\n    is worth honouring, because it is the opposite of the FundzWatch surface on the same host.\n- id: oauthBearer\n  surface: core\n  type: http\n  scheme: bearer\n  in: header\n  name: Authorization\n  source: https://app.fundz.net/knowledge/api-references/authentication\n  in_openapi: false\n  description: >-\n    \"For ChatGPT and other agent integrations, the API also accepts an OAuth access token using the\n    Bearer scheme: Authorization: Bearer <access_token>.\" No authorization endpoint, token\n    endpoint, client registration or scope list is published, and\n    /.well-known/oauth-authorization-server 404s on every host\
  \ — so this is an accepted credential\n    format rather than a documented OAuth 2.0 deployment. No scopes/ artifact was written for\n    exactly this reason.\n- id: sessionCookie\n  surface: in-app browser\n  type: cookie\n  source: https://app.fundz.net/knowledge/api-references/authentication\n  description: In-app browser usage is authenticated by a logged-in session cookie. Not for programmatic use.\n- id: fundzwatchBearer\n  surface: fundzwatch\n  type: http\n  scheme: bearer\n  in: header\n  name: Authorization\n  base: https://api.fundz.net/v1/watch\n  source: https://fundzwatch.ai/docs\n  in_openapi: false\n  key_prefixes:\n  - {prefix: fundz_test_, mode: test, note: 'Developer-tier limits, live data.'}\n  - {prefix: fundz_live_, mode: live, note: Paid plans.}\n  example: 'curl https://api.fundz.net/v1/watch/events -H \"Authorization: Bearer YOUR_API_KEY\"'\n  environment_variable: FUNDZWATCH_API_KEY\n  description: >-\n    Prefixed, mode-separated keys with a Bearer scheme — a\
  \ materially more modern auth posture than\n    the core API's raw header, on the same hostname.\naccess:\n  core_api:\n    free_tier: false\n    card_required: true\n    instant: false\n    statement: >-\n      \"The Fundz API is available on paid plans only — there is no free API tier.\" Subscribe to Pro\n      or Strategic, then request the key from your account or support@fundz.net.\n    source: https://app.fundz.net/knowledge/api-references/authentication\n    correction: >-\n      CORRECTED 2026-08-14. A prior pass recorded \"a free key is issued instantly, with no card and\n      no sales call\" from the https://www.fundz.net/api-trial page and treated it as the core API's\n      access model. The API reference states the opposite for the core API. The free instant key is\n      real, but it is the FUNDZWATCH developer key (fundz_test_), which authorizes /v1/watch/* and\n      the MCP server — not GET /fundings. The distinction matters: the differentiator Fundz leads\n      with\
  \ against Crunchbase applies to its agent surface, not to its feed API.\n  fundzwatch_api:\n    free_tier: true\n    plan: Developer (Free)\n    card_required: false\n    instant: true\n    signup: https://fundzwatch.ai/onboarding\n    alt_signup: https://www.fundz.net/api-trial\n    limits: {api_calls_per_month: 1000, ai_score_calls_per_month: 100}\n  mcp:\n    key_required: false\n    note: 7 of the 14 MCP tools return live data with no credential at all.\nfailure_modes:\n- {status: 401, meaning: 'Authentication required, invalid token, or subscription inactive — the message points at fundz.net/pricing.', source: docs}\n- {status: 403, meaning: 'Missing, invalid, orphaned or non-entitled API key.', source: openapi, observed: '{\"type\":\"Unauthorized\",\"message\":\"Authentication required\"}'}\n- {status: 403, meaning: 'On /fund-formations, a non-subscriber receives {\"error\": \"subscription_required\"}.', source: 'https://app.fundz.net/knowledge/api-references/fund-formations'}\n\
  transport_security:\n  https_only: true\n  tls_version: TLSv1.3\n  hsts: false\n  note: >-\n    HSTS is NOT set on api.fundz.net or www.fundz.net — see security/fundz-domain-security.yml. For\n    an API whose only credential is a bearer-equivalent header value, that is the most consequential\n    gap in the auth posture.\nevidence:\n- {url: 'https://app.fundz.net/knowledge/api-references/authentication', status: 200}\n- {url: 'https://app.fundz.net/knowledge/api-references/companies', status: 200}\n- {url: 'https://fundzwatch.ai/docs', status: 200}\n- {url: 'https://api.fundz.net/fundings', status: 403, note: 'live probe, no credential'}\n- {url: 'https://api.fundz.net/.well-known/oauth-authorization-server', status: 404}\n- {url: 'https://www.fundz.net/api-trial', status: 200}\ngaps:\n- Bearer/OAuth is accepted but no authorization server, token endpoint or scopes are published.\n- No key rotation, expiry or revocation policy documented.\n- No HSTS on the API host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fundz/refs/heads/main/authentication/fundz-authentication.yml
summary_line: apiKey/http-bearer · 4 schemes
tags:
- Business Intelligence
- Funding
- Private Markets
- Mergers and Acquisitions
- SEC Filings
- Signals
- Sales Intelligence
- MCP
- Agents
---
