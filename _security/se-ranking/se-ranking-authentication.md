---
api_key_in:
- header
- query
api_specs:
- filename: overview
  format: yaml
  label: SE Ranking Data API
  slug: data-api
  spec_type: Postman
  url: https://www.postman.com/serankingdev/se-ranking-developers/overview
- filename: overview
  format: yaml
  label: SE Ranking Project API
  slug: project-api
  spec_type: Postman
  url: https://www.postman.com/serankingdev/se-ranking-developers/overview
- filename: se-ranking-account-system-api-openapi.yml
  format: yaml
  label: SE Ranking Account & system API
  slug: se-ranking-account-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/se-ranking/refs/heads/main/openapi/se-ranking-account-system-api-openapi.yml
- filename: se-ranking-ai-search-api-openapi.yml
  format: yaml
  label: SE Ranking AI search API
  slug: se-ranking-ai-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/se-ranking/refs/heads/main/openapi/se-ranking-ai-search-api-openapi.yml
- filename: se-ranking-backlinks-api-openapi.yml
  format: yaml
  label: SE Ranking backlinks API
  slug: se-ranking-backlinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/se-ranking/refs/heads/main/openapi/se-ranking-backlinks-api-openapi.yml
- filename: se-ranking-domain-analysis-api-openapi.yml
  format: yaml
  label: SE Ranking Domain Analysis API
  slug: se-ranking-domain-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/se-ranking/refs/heads/main/openapi/se-ranking-domain-analysis-api-openapi.yml
- filename: se-ranking-keyword-research-api-openapi.yml
  format: yaml
  label: SE Ranking Keyword Research API
  slug: se-ranking-keyword-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/se-ranking/refs/heads/main/openapi/se-ranking-keyword-research-api-openapi.yml
- filename: se-ranking-serp-results-classic-api-openapi.yml
  format: yaml
  label: SE Ranking SERP Results > classic API
  slug: se-ranking-serp-results-classic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/se-ranking/refs/heads/main/openapi/se-ranking-serp-results-classic-api-openapi.yml
- filename: se-ranking-website-audit-api-openapi.yml
  format: yaml
  label: SE Ranking Website Audit API
  slug: se-ranking-website-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/se-ranking/refs/heads/main/openapi/se-ranking-website-audit-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Se Ranking Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: SE Ranking secures its APIs with apiKey and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: SE Ranking
provider_slug: se-ranking
scheme_count: 4
schemes:
- in: query
  name: apikeyAuth
  note: The only scheme the published OpenAPI declares. SE Ranking's own docs discourage it in production because the key leaks into access logs, browser history and referrers.
  parameter: apikey
  sources:
  - openapi/_original/se-ranking-data-api-openapi.yml
  surface: REST (Data API + Project API)
  type: apiKey
- in: header
  name: authorizationTokenHeader
  note: 'Recommended REST form: `Authorization: Token YOUR_API_KEY`. The scheme prefix is `Token`, NOT `Bearer` — a Bearer prefix on the REST API is a 401. Not declared in the OpenAPI, which is a spec/docs gap.'
  parameter: Authorization
  recommended: true
  sources:
  - https://seranking.com/api/data/getting-started/
  - https://github.com/seranking/seo-skills/blob/main/skills/seo-api/references/auth-and-keys.md
  surface: REST (Data API + Project API)
  type: apiKey
  value_prefix: 'Token '
- aliases:
  - X-Data-Api-Key
  in: header
  name: mcpApiKeyHeader
  note: Non-interactive/CI auth for the MCP server. Header auth takes precedence over an existing OAuth Bearer token.
  parameter: X-Api-Key
  sources:
  - https://seranking.com/api/mcp/
  - https://github.com/seranking/seo-skills/blob/main/skills/seo-api/references/auth-and-keys.md
  surface: MCP (https://api.seranking.com/mcp)
  type: apiKey
- flows:
  - authorizationUrl: https://seranking.com/wp-json/seranking-mcp-oauth/v1/authorize
    dynamic_client_registration: https://seranking.com/wp-json/seranking-mcp-oauth/v1/register
    flow: authorizationCode
    pkce: S256
    scopes:
    - mcp
    tokenUrl: https://seranking.com/wp-json/seranking-mcp-oauth/v1/token
  name: mcpOAuth
  note: OAuth 2.1 + PKCE + RFC 7591 dynamic client registration. Refresh token is a 30-day sliding window per SE Ranking's published skill reference. See scopes/se-ranking-scopes.yml.
  sources:
  - https://seranking.com/.well-known/oauth-authorization-server
  - https://seranking.com/.well-known/oauth-protected-resource
  surface: MCP (https://api.seranking.com/mcp)
  type: oauth2
slug: se-ranking-authentication
source_filename: se-ranking-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/_original/se-ranking-data-api-openapi.yml + https://seranking.com/api/data/getting-started/ + https://seranking.com/api/mcp/\n  + https://github.com/seranking/seo-skills/blob/main/skills/seo-api/references/auth-and-keys.md\ndocs: https://seranking.com/api/data/getting-started/\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  - query\n  oauth2_flows:\n  - authorizationCode\n  note: 'One API key authenticates every surface as of 2026 — the legacy split into separate Data and Project keys is retired (source:\n    SE Ranking seo-api skill reference auth-and-keys.md). Keys are UUID-shaped and minted in the API Dashboard.'\nschemes:\n- name: apikeyAuth\n  type: apiKey\n  in: query\n  parameter: apikey\n  surface: REST (Data API + Project API)\n  sources:\n  - openapi/_original/se-ranking-data-api-openapi.yml\n  note: The only scheme the published OpenAPI declares. SE Ranking's own docs discourage\
  \ it in production because the key leaks into\n    access logs, browser history and referrers.\n- name: authorizationTokenHeader\n  type: apiKey\n  in: header\n  parameter: Authorization\n  surface: REST (Data API + Project API)\n  value_prefix: 'Token '\n  recommended: true\n  sources:\n  - https://seranking.com/api/data/getting-started/\n  - https://github.com/seranking/seo-skills/blob/main/skills/seo-api/references/auth-and-keys.md\n  note: 'Recommended REST form: `Authorization: Token YOUR_API_KEY`. The scheme prefix is `Token`, NOT `Bearer` — a Bearer prefix on\n    the REST API is a 401. Not declared in the OpenAPI, which is a spec/docs gap.'\n- name: mcpApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  surface: MCP (https://api.seranking.com/mcp)\n  aliases:\n  - X-Data-Api-Key\n  sources:\n  - https://seranking.com/api/mcp/\n  - https://github.com/seranking/seo-skills/blob/main/skills/seo-api/references/auth-and-keys.md\n  note: Non-interactive/CI auth for the\
  \ MCP server. Header auth takes precedence over an existing OAuth Bearer token.\n- name: mcpOAuth\n  type: oauth2\n  surface: MCP (https://api.seranking.com/mcp)\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://seranking.com/wp-json/seranking-mcp-oauth/v1/authorize\n    tokenUrl: https://seranking.com/wp-json/seranking-mcp-oauth/v1/token\n    scopes:\n    - mcp\n    pkce: S256\n    dynamic_client_registration: https://seranking.com/wp-json/seranking-mcp-oauth/v1/register\n  sources:\n  - https://seranking.com/.well-known/oauth-authorization-server\n  - https://seranking.com/.well-known/oauth-protected-resource\n  note: OAuth 2.1 + PKCE + RFC 7591 dynamic client registration. Refresh token is a 30-day sliding window per SE Ranking's published\n    skill reference. See scopes/se-ranking-scopes.yml.\nanonymous_surface:\n  endpoint: https://api.seranking.com/mcp\n  methods:\n  - tools/list\n  - prompts/list\n  note: 'Probed 2026-08-13: tools/list and prompts/list return\
  \ HTTP 200 with the full manifest WITHOUT credentials. initialize and every\n    tools/call require a token. Discovery is open; execution is not.'\nkey_management:\n  dashboard: https://online.seranking.com/admin.api.dashboard.html\n  multiple_keys: true\n  rotation_note: Keys are cached server-side; allow up to 60 seconds after revocation before treating an old key as dead (SE Ranking\n    published guidance).\n  liveness_check: GET https://api.seranking.com/v1/account/subscription (0 credits)\nplan_gating:\n  data_api: Any plan carrying API credits.\n  project_api: Business or Enterprise only — otherwise 403 Subscription required.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/se-ranking/refs/heads/main/authentication/se-ranking-authentication.yml
summary_line: apiKey/oauth2 · 4 schemes
tags:
- SEO
- Keyword Research
- Rank Tracking
- Backlinks
- Competitor Analysis
- Website Audit
- AI Search
- GEO
- Digital Marketing
- MCP
- AI Agents
- Agent Skills
---
