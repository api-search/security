---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: mrscraper-analytic-api-openapi.yml
  format: yaml
  label: MrScraper Analytic API
  slug: mrscraper-analytic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/openapi/mrscraper-analytic-api-openapi.yml
- filename: mrscraper-auth-api-openapi.yml
  format: yaml
  label: MrScraper Auth API
  slug: mrscraper-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/openapi/mrscraper-auth-api-openapi.yml
- filename: mrscraper-gateway-api-openapi.yml
  format: yaml
  label: MrScraper Gateway API
  slug: mrscraper-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/openapi/mrscraper-gateway-api-openapi.yml
- filename: mrscraper-jobs-api-openapi.yml
  format: yaml
  label: MrScraper Jobs API
  slug: mrscraper-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/openapi/mrscraper-jobs-api-openapi.yml
- filename: mrscraper-proxies-api-openapi.yml
  format: yaml
  label: MrScraper Proxies API
  slug: mrscraper-proxies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/openapi/mrscraper-proxies-api-openapi.yml
- filename: mrscraper-results-api-openapi.yml
  format: yaml
  label: MrScraper Results API
  slug: mrscraper-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/openapi/mrscraper-results-api-openapi.yml
- filename: mrscraper-storage-api-openapi.yml
  format: yaml
  label: MrScraper Storage API
  slug: mrscraper-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/openapi/mrscraper-storage-api-openapi.yml
- filename: mrscraper-tasks-api-openapi.yml
  format: yaml
  label: MrScraper Tasks API
  slug: mrscraper-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/openapi/mrscraper-tasks-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Mrscraper Authentication
name_suffix: Authentication
oauth_flows: []
overview: MrScraper secures its APIs with apiKey and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MrScraper
provider_slug: mrscraper
scheme_count: 4
schemes:
- description: MrScraper API token created at https://app.mrscraper.com/api-tokens (name + expiration date). Required on every Platform API and Scraper API request. Analytics endpoints accept an `apiTokenName` query filter.
  docs: https://docs.mrscraper.com/docs/getting-started/api-token
  in: header
  name: ApiKeyAuth
  parameter: x-api-token
  sources:
  - https://docs.mrscraper.com/docs/api/authentication
  - openapi/mrscraper-scraper-service-gateway-openapi.yml
  type: apiKey
- description: '"Authorization: Bearer <token>" - the same MrScraper API token for Marketplace endpoints (RFC 6750), or an OAuth 2.1 access token issued by the platform for the MCP connector.'
  name: BearerAuth
  scheme: bearer
  sources:
  - https://docs.mrscraper.com/docs/api/authentication
  - openapi/mrscraper-scraper-service-gateway-openapi.yml
  type: http
- description: The Scraper API (GET https://api.mrscraper.com/?url=...) also accepts the API token as a `token` query parameter, as shown on the Response Headers page.
  in: query
  name: TokenQuery
  parameter: token
  sources:
  - https://docs.mrscraper.com/docs/api/response-headers
  - openapi/mrscraper-scraper-service-gateway-openapi.yml
  type: apiKey
- description: OAuth 2.1 for the hosted MCP endpoint https://mcp.mrscraper.com/mcp - RFC 9728 protected-resource metadata, RFC 8414 authorization-server metadata, PKCE S256, dynamic client registration, refresh tokens. A tool called without its scope returns 403 insufficient_scope.
  flows:
    authorizationCode:
      authorizationUrl: https://api.app.mrscraper.com/oauth/authorize
      refreshUrl: https://api.app.mrscraper.com/oauth/token
      scopes:
        account:read: status
        offline_access: refresh token
        scrape:read: fetch, serp, results, result
        scrape:write: scrape, rerun
      tokenUrl: https://api.app.mrscraper.com/oauth/token
  name: McpOAuth
  sources:
  - https://mcp.mrscraper.com/.well-known/oauth-protected-resource/mcp
  - https://api.app.mrscraper.com/.well-known/oauth-authorization-server
  - https://docs.mrscraper.com/docs/getting-started/mcp-server
  type: oauth2
slug: mrscraper-authentication
source_filename: mrscraper-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: searched\nsource: https://docs.mrscraper.com/docs/api/authentication\ndocs: https://docs.mrscraper.com/docs/api/authentication\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header, query]\n  note: Every REST endpoint takes a MrScraper API token in the x-api-token header; Marketplace endpoints take the same token as an RFC 6750 Bearer; the Scraper API also accepts the token as a `token` query parameter. The hosted MCP server is OAuth 2.1 (authorization code + PKCE) with an API-key Bearer fallback.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-token\n  description: MrScraper API token created at https://app.mrscraper.com/api-tokens (name + expiration date). Required on every Platform API and Scraper API request. Analytics endpoints accept an `apiTokenName` query filter.\n  docs: https://docs.mrscraper.com/docs/getting-started/api-token\n  sources:\n  - https://docs.mrscraper.com/docs/api/authentication\n\
  \  - openapi/mrscraper-scraper-service-gateway-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: '\"Authorization: Bearer <token>\" - the same MrScraper API token for Marketplace endpoints (RFC 6750), or an OAuth 2.1 access token issued by the platform for the MCP connector.'\n  sources:\n  - https://docs.mrscraper.com/docs/api/authentication\n  - openapi/mrscraper-scraper-service-gateway-openapi.yml\n- name: TokenQuery\n  type: apiKey\n  in: query\n  parameter: token\n  description: The Scraper API (GET https://api.mrscraper.com/?url=...) also accepts the API token as a `token` query parameter, as shown on the Response Headers page.\n  sources:\n  - https://docs.mrscraper.com/docs/api/response-headers\n  - openapi/mrscraper-scraper-service-gateway-openapi.yml\n- name: McpOAuth\n  type: oauth2\n  description: OAuth 2.1 for the hosted MCP endpoint https://mcp.mrscraper.com/mcp - RFC 9728 protected-resource metadata, RFC 8414 authorization-server metadata, PKCE\
  \ S256, dynamic client registration, refresh tokens. A tool called without its scope returns 403 insufficient_scope.\n  flows:\n    authorizationCode:\n      authorizationUrl: https://api.app.mrscraper.com/oauth/authorize\n      tokenUrl: https://api.app.mrscraper.com/oauth/token\n      refreshUrl: https://api.app.mrscraper.com/oauth/token\n      scopes:\n        scrape:read: fetch, serp, results, result\n        scrape:write: scrape, rerun\n        account:read: status\n        offline_access: refresh token\n  sources:\n  - https://mcp.mrscraper.com/.well-known/oauth-protected-resource/mcp\n  - https://api.app.mrscraper.com/.well-known/oauth-authorization-server\n  - https://docs.mrscraper.com/docs/getting-started/mcp-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/authentication/mrscraper-authentication.yml
summary_line: apiKey/oauth2 · 4 schemes
tags:
- Company
- Web Scraping
- Data Extraction
- Proxies
- AI Agents
- MCP
- Search
- Browser Automation
---
