---
api_key_in:
- header
api_specs:
- filename: caplight-companies-api-openapi.yml
  format: yaml
  label: Caplight Companies API
  slug: caplight-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-companies-api-openapi.yml
- filename: caplight-company-api-openapi.yml
  format: yaml
  label: Caplight Company API
  slug: caplight-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-company-api-openapi.yml
- filename: caplight-company-details-api-openapi.yml
  format: yaml
  label: Caplight Company Details API
  slug: caplight-company-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-company-details-api-openapi.yml
- filename: caplight-company-filings-api-openapi.yml
  format: yaml
  label: Caplight Company Filings API
  slug: caplight-company-filings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-company-filings-api-openapi.yml
- filename: caplight-company-lookup-api-openapi.yml
  format: yaml
  label: Caplight Company Lookup API
  slug: caplight-company-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-company-lookup-api-openapi.yml
- filename: caplight-composite-index-api-openapi.yml
  format: yaml
  label: Caplight Composite Index API
  slug: caplight-composite-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-composite-index-api-openapi.yml
- filename: caplight-comps-api-openapi.yml
  format: yaml
  label: Caplight Comps API
  slug: caplight-comps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-comps-api-openapi.yml
- filename: caplight-fund-marks-api-openapi.yml
  format: yaml
  label: Caplight Fund Marks API
  slug: caplight-fund-marks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-fund-marks-api-openapi.yml
- filename: caplight-funding-rounds-api-openapi.yml
  format: yaml
  label: Caplight Funding Rounds API
  slug: caplight-funding-rounds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-funding-rounds-api-openapi.yml
- filename: caplight-investors-api-openapi.yml
  format: yaml
  label: Caplight Investors API
  slug: caplight-investors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-investors-api-openapi.yml
- filename: caplight-live-orderbook-api-openapi.yml
  format: yaml
  label: Caplight Live Orderbook API
  slug: caplight-live-orderbook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-live-orderbook-api-openapi.yml
- filename: caplight-marketprice-api-openapi.yml
  format: yaml
  label: Caplight Market Price API
  slug: caplight-marketprice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-marketprice-api-openapi.yml
- filename: caplight-news-api-openapi.yml
  format: yaml
  label: Caplight News API
  slug: caplight-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-news-api-openapi.yml
- filename: caplight-order-history-api-openapi.yml
  format: yaml
  label: Caplight Order History API
  slug: caplight-order-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-order-history-api-openapi.yml
- filename: caplight-stock-splits-api-openapi.yml
  format: yaml
  label: Caplight Stock Splits API
  slug: caplight-stock-splits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-stock-splits-api-openapi.yml
- filename: caplight-trade-history-api-openapi.yml
  format: yaml
  label: Caplight Trade History API
  slug: caplight-trade-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-trade-history-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Caplight Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Caplight secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Caplight
provider_slug: caplight
scheme_count: 2
schemes:
- description: Caplight API authentication is managed through an api_key header value. Please contact us if you do not yet have an API key. API access is a paid add-on to Caplight Data; keys are issued on request to contact@caplight.com.
  in: header
  name: api_key
  parameter: api_key
  sources:
  - openapi/caplight-rest-api-openapi-original.json
  surface: Caplight REST API
  type: apiKey
  x-evidence:
    body: '{"message":"Invalid/missing API key. Please set request header api_key with your provided API key"}'
    fetched: '2026-08-09'
    http_status: 401
    url: https://us-central1-caplight-prod.cloudfunctions.net/api/public/v1/companies?domain=stripe.com
- bearer_methods_supported:
  - header
  description: OAuth 2.1 authorization-code flow protecting https://platform.caplight.com/mcp. Advertised through RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata. Bearer token in the Authorization header. No scopes are advertised in the metadata document.
  flows:
  - authorizationUrl: https://platform.caplight.com/mcp/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    registrationUrl: https://platform.caplight.com/mcp/register
    scopes: []
    tokenUrl: https://platform.caplight.com/mcp/token
  name: mcp_oauth
  sources:
  - well-known/caplight-oauth-authorization-server.json
  - well-known/caplight-oauth-protected-resource.json
  surface: Caplight MCP Server
  type: oauth2
  x-evidence:
    body: '{"error":"Unauthorized","message":"Valid authentication required. Use the OAuth flow to obtain an access token."}'
    fetched: '2026-08-09'
    http_status: 401
    url: https://platform.caplight.com/mcp
slug: caplight-authentication
source_filename: caplight-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: openapi/caplight-rest-api-openapi-original.json\ndocs: https://platform.caplight.com/api/documentation.html\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  notes: >-\n    Two independent auth models across two surfaces. The REST API uses a static api_key request header\n    (no OAuth, no scopes). The hosted MCP server uses OAuth 2.1 authorization code + PKCE with dynamic\n    client registration, and explicitly requires no API key — a Caplight account is the credential.\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: api_key\n  surface: Caplight REST API\n  description: >-\n    Caplight API authentication is managed through an api_key header value. Please contact us if you do\n    not yet have an API key. API access is a paid add-on to Caplight Data; keys are issued on request to\n    contact@caplight.com.\n  sources:\n  - openapi/caplight-rest-api-openapi-original.json\n\
  \  x-evidence:\n    fetched: '2026-08-09'\n    url: https://us-central1-caplight-prod.cloudfunctions.net/api/public/v1/companies?domain=stripe.com\n    http_status: 401\n    body: '{\"message\":\"Invalid/missing API key. Please set request header api_key with your provided API key\"}'\n- name: mcp_oauth\n  type: oauth2\n  surface: Caplight MCP Server\n  description: >-\n    OAuth 2.1 authorization-code flow protecting https://platform.caplight.com/mcp. Advertised through\n    RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata. Bearer token in the\n    Authorization header. No scopes are advertised in the metadata document.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform.caplight.com/mcp/authorize\n    tokenUrl: https://platform.caplight.com/mcp/token\n    registrationUrl: https://platform.caplight.com/mcp/register\n    grant_types:\n    - authorization_code\n    - refresh_token\n    code_challenge_methods:\n    - S256\n    scopes:\
  \ []\n  bearer_methods_supported:\n  - header\n  sources:\n  - well-known/caplight-oauth-authorization-server.json\n  - well-known/caplight-oauth-protected-resource.json\n  x-evidence:\n    fetched: '2026-08-09'\n    url: https://platform.caplight.com/mcp\n    http_status: 401\n    body: '{\"error\":\"Unauthorized\",\"message\":\"Valid authentication required. Use the OAuth flow to obtain an access token.\"}'\nauthorization:\n  model: per-account entitlements\n  description: >-\n    Beyond authentication, v2 company-scoped endpoints enforce per-account access control documented in\n    the OpenAPI description: an optional whitelist of permitted companies, an optional annual cap on\n    distinct companies accessed (repeat access to the same company counts once), and field-level\n    restrictions. When a field is restricted it is omitted from the response and named in the\n    restricted.fields array on the funding round object. Restricted fields may include amounts,\n    valuation, pps,\
  \ participants and citations.\n  error_codes:\n  - status: 401\n    meaning: Missing or invalid API key\n  - status: 403\n    meaning: >-\n      Account does not have Companies V2 API access, or the company is outside the whitelist / over the\n      annual cap\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/authentication/caplight-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Private Markets
- Secondary Market
- Market Data
- Venture Capital
- Company Data
- investor-data
- Funding Rounds
- Pricing Data
- Financial Data
- Fintech
- MCP
- agent-native
---
