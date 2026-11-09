---
anonymous_access: true
api_key_in: []
api_specs:
- filename: fin-discovery-com-call-tool-api-openapi.yml
  format: yaml
  label: Fintel Discovery Call Tool API
  slug: fin-discovery-com-call-tool-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fin-discovery-com/openapi/fin-discovery-com-call-tool-api-openapi.yml
- filename: fin-discovery-com-fastapi-api-openapi.yml
  format: yaml
  label: Fintel Discovery Fast API
  slug: fin-discovery-com-fastapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fin-discovery-com/openapi/fin-discovery-com-fastapi-api-openapi.yml
- filename: fin-discovery-com-getatoken-api-openapi.yml
  format: yaml
  label: Fintel Discovery Get A Token API
  slug: fin-discovery-com-getatoken-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fin-discovery-com/openapi/fin-discovery-com-getatoken-api-openapi.yml
- filename: fin-discovery-com-login-api-openapi.yml
  format: yaml
  label: Fintel Discovery Login API
  slug: fin-discovery-com-login-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fin-discovery-com/openapi/fin-discovery-com-login-api-openapi.yml
- filename: fin-discovery-com-tool-endpoint-api-openapi.yml
  format: yaml
  label: Fintel Discovery Tool Endpoint API
  slug: fin-discovery-com-tool-endpoint-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fin-discovery-com/openapi/fin-discovery-com-tool-endpoint-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Fin Discovery Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fintel Discovery declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Fintel Discovery
provider_slug: fin-discovery-com
scheme_count: 3
schemes:
- evidence: '"Authentication: None required" on https://fin-discovery.com/'
  scope: MCP server and all non-FRED/non-Census tools
  type: none
- evidence: '"FRED tools require a free FRED API key" on https://fin-discovery.com/docs/api.html'
  scope: SearchFredSeries, GetFredSeriesData (optional FRED API key)
  type: user-supplied-upstream-key
- evidence: '"Free Census API key (api.census.gov/data/key_signup.html). Falls back to rate-limited access if omitted." on https://fin-discovery.com/docs/api.html'
  scope: GetTerritoryWealthProfile (optional Census API key)
  type: user-supplied-upstream-key
slug: fin-discovery-com-authentication
source_filename: fin-discovery-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://fin-discovery.com/\ndocs: https://fin-discovery.com/docs/api.html\nname: Fintel Discovery authentication\nsummary: >-\n  The Fintel Discovery MCP server is public. The homepage's Technical\n  Specifications block states \"Authentication: None required\" for the MCP\n  endpoint at https://ai.fin-discovery.com/mcp, and the docs' Tool Reference\n  says \"0 API keys required*\" with a footnote that the FRED-backed tools\n  (SearchFredSeries, GetFredSeriesData) accept an optional caller-provided FRED\n  API key and the Census tool (GetTerritoryWealthProfile) accepts an optional\n  caller-provided Census API key; without them those specific tools fall back\n  to rate-limited public access.\nschemes:\n  - type: none\n    scope: MCP server and all non-FRED/non-Census tools\n    evidence: '\"Authentication: None required\" on https://fin-discovery.com/'\n  - type: user-supplied-upstream-key\n    scope: SearchFredSeries, GetFredSeriesData\
  \ (optional FRED API key)\n    evidence: '\"FRED tools require a free FRED API key\" on https://fin-discovery.com/docs/api.html'\n  - type: user-supplied-upstream-key\n    scope: GetTerritoryWealthProfile (optional Census API key)\n    evidence: '\"Free Census API key (api.census.gov/data/key_signup.html). Falls back to rate-limited access if omitted.\" on https://fin-discovery.com/docs/api.html'\nnotes: >-\n  The published OpenAPI at https://ai.fin-discovery.com/openapi.json describes\n  a FastAPI wrapper that exposes /login and /getAToken paths. These were NOT\n  probed (safety rule: never GET /login or /token). The public-facing surface\n  advertised on the website is unauthenticated MCP; any login flow in the\n  OpenAPI is undocumented on the website and is not represented to end users.\n"
source_yaml_url: https://artifacts.apis.io/fin-discovery-com/authentication/fin-discovery-com-authentication.yml
summary_line: 3 schemes
tags:
- Financial Services
- Regulatory Data
- Broker Check
- SEC EDGAR
- Market Data
- MCP Server
- AI Agents
- Compliance
---
