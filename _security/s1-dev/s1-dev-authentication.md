---
anonymous_access: false
api_key_in: []
api_specs:
- filename: s1-dev-account-api-openapi.yml
  format: yaml
  label: Search1API Account API
  slug: s1-dev-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s1-dev/refs/heads/main/openapi/s1-dev-account-api-openapi.yml
- filename: s1-dev-crawl-api-openapi.yml
  format: yaml
  label: Search1API Crawl API
  slug: s1-dev-crawl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s1-dev/refs/heads/main/openapi/s1-dev-crawl-api-openapi.yml
- filename: s1-dev-feedback-api-openapi.yml
  format: yaml
  label: Search1API Feedback API
  slug: s1-dev-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s1-dev/refs/heads/main/openapi/s1-dev-feedback-api-openapi.yml
- filename: s1-dev-screenshot-api-openapi.yml
  format: yaml
  label: Search1API Screenshot API
  slug: s1-dev-screenshot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s1-dev/refs/heads/main/openapi/s1-dev-screenshot-api-openapi.yml
- filename: s1-dev-search-api-openapi.yml
  format: yaml
  label: Search1API Search API
  slug: s1-dev-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s1-dev/refs/heads/main/openapi/s1-dev-search-api-openapi.yml
- filename: s1-dev-system-api-openapi.yml
  format: yaml
  label: Search1API System API
  slug: s1-dev-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s1-dev/refs/heads/main/openapi/s1-dev-system-api-openapi.yml
auth_types:
- http
- oauth2
- payment-challenge
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: S1 Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Search1API secures its APIs with http, oauth2, and payment-challenge across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Search1API
provider_slug: s1-dev
scheme_count: 3
schemes:
- bearerFormat: API Key
  description: 'User-managed API key created in https://app.s1.dev, sent as Authorization: Bearer. The hosted MCP server also accepts ?apiKey= for clients that cannot send headers (header wins).'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/s1-dev-openapi.yml
  type: http
- description: 'OAuth 2.1 for agents, OAuth-aware MCP clients and the s1 CLI: dynamic client registration, authorization code + PKCE S256, refresh with offline_access. Discovery starts at the protected-resource metadata (RFC 9728) of api.search1api.com or mcp.search1api.com.'
  flows:
    authorizationCode:
      authorizationUrl: https://clerk.s1.dev/oauth/authorize
      refreshUrl: https://clerk.s1.dev/oauth/token
      scopes:
        offline_access: refresh token
        openid: identity
      tokenUrl: https://clerk.s1.dev/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  issuer: https://clerk.s1.dev
  name: oauth2
  pkce:
  - S256
  protected_resources:
  - https://api.search1api.com
  - https://mcp.search1api.com/mcp
  registration_endpoint: https://clerk.s1.dev/oauth/register
  revocation_endpoint: https://clerk.s1.dev/oauth/token/revoke
  sources:
  - https://s1.dev/auth.md
  type: oauth2
- description: 'Pay-per-request: a call without a bearer token receives 402 application/problem+json with a WWW-Authenticate: Payment challenge (MPP, method="tempo"); the spec names MPP and x402.'
  name: paymentChallenge
  sources:
  - https://s1.dev/docs/essentials/error-handling
  - live POST https://api.search1api.com/search 2026-10-07
  type: payment
slug: s1-dev-authentication
source_filename: s1-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: searched\nsource: https://s1.dev/docs/essentials/authentication; https://s1.dev/auth.md; https://clerk.s1.dev/.well-known/oauth-authorization-server;\n  openapi/s1-dev-openapi.yml\ndocs: https://s1.dev/docs/essentials/authentication\nsummary:\n  types:\n  - http\n  - oauth2\n  - payment-challenge\n  header: 'Authorization: Bearer <token-or-key>'\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: 'User-managed API key created in https://app.s1.dev, sent as Authorization: Bearer. The hosted MCP\n    server also accepts ?apiKey= for clients that cannot send headers (header wins).'\n  sources:\n  - openapi/s1-dev-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n    authorizationCode:\n      authorizationUrl: https://clerk.s1.dev/oauth/authorize\n      tokenUrl: https://clerk.s1.dev/oauth/token\n      refreshUrl: https://clerk.s1.dev/oauth/token\n      scopes:\n        openid: identity\n \
  \       offline_access: refresh token\n  issuer: https://clerk.s1.dev\n  registration_endpoint: https://clerk.s1.dev/oauth/register\n  revocation_endpoint: https://clerk.s1.dev/oauth/token/revoke\n  pkce:\n  - S256\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  description: 'OAuth 2.1 for agents, OAuth-aware MCP clients and the s1 CLI: dynamic client registration, authorization\n    code + PKCE S256, refresh with offline_access. Discovery starts at the protected-resource metadata (RFC 9728)\n    of api.search1api.com or mcp.search1api.com.'\n  protected_resources:\n  - https://api.search1api.com\n  - https://mcp.search1api.com/mcp\n  sources:\n  - https://s1.dev/auth.md\n- name: paymentChallenge\n  type: payment\n  description: 'Pay-per-request: a call without a bearer token receives 402 application/problem+json with a WWW-Authenticate:\n    Payment challenge (MPP, method=\"tempo\"); the spec names MPP and x402.'\n  sources:\n\
  \  - https://s1.dev/docs/essentials/error-handling\n  - live POST https://api.search1api.com/search 2026-10-07\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/s1-dev/refs/heads/main/authentication/s1-dev-authentication.yml
summary_line: http/oauth2/payment-challenge · 3 schemes
tags:
- Company
- Search
- Web Search
- Crawling
- Web Scraping
- News
- AI Agents
- MCP
- Agent Tools
- Data Extraction
- Screenshots
---
