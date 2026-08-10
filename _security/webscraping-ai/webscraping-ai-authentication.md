---
api_key_in:
- query
api_specs:
- filename: webscraping-ai-account-api-openapi.yml
  format: yaml
  label: WebScraping.AI Account API
  slug: webscraping-ai-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webscraping-ai/refs/heads/main/openapi/webscraping-ai-account-api-openapi.yml
- filename: webscraping-ai-ai-api-openapi.yml
  format: yaml
  label: WebScraping.AI AI API
  slug: webscraping-ai-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webscraping-ai/refs/heads/main/openapi/webscraping-ai-ai-api-openapi.yml
- filename: webscraping-ai-html-api-openapi.yml
  format: yaml
  label: WebScraping.AI HTML API
  slug: webscraping-ai-html-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webscraping-ai/refs/heads/main/openapi/webscraping-ai-html-api-openapi.yml
- filename: webscraping-ai-selected-html-api-openapi.yml
  format: yaml
  label: WebScraping.AI Selected HTML API
  slug: webscraping-ai-selected-html-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webscraping-ai/refs/heads/main/openapi/webscraping-ai-selected-html-api-openapi.yml
- filename: webscraping-ai-text-api-openapi.yml
  format: yaml
  label: WebScraping.AI Text API
  slug: webscraping-ai-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webscraping-ai/refs/heads/main/openapi/webscraping-ai-text-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Webscraping Ai Authentication
name_suffix: Authentication
oauth_flows:
- authorization_code
overview: WebScraping.AI secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorization_code flow(s).
provider_name: WebScraping.AI
provider_slug: webscraping-ai
scheme_count: 3
schemes:
- applies_to: https://api.webscraping.ai
  description: All REST API requests require an API key passed as the `api_key` query-string parameter. There is no header form documented. The docs warn the key must not be exposed in client-side code.
  in: query
  name: api_key
  parameter: api_key
  sources:
  - openapi/webscraping-ai-openapi.yml
  - https://webscraping.ai/docs
  type: apiKey
- applies_to: http://proxy.webscraping.ai:8888
  description: Proxy Mode (proxy.webscraping.ai:8888) authenticates with HTTP proxy credentials — the username is the API key and the password carries the request parameters (e.g. `js=true&proxy=residential`). The proxy presents a self-signed certificate.
  name: proxy_basic_auth
  scheme: basic
  sources:
  - https://webscraping.ai/docs
  type: http
- description: 'The hosted remote MCP server (https://mcp.webscraping.ai/mcp) is protected by OAuth 2.1 with PKCE and dynamic client registration — no API key is used. Anonymous requests are rejected with 401 and a RFC 9728 `WWW-Authenticate: Bearer resource_metadata=...` challenge.'
  flows:
  - authorizationUrl: https://webscraping.ai/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    registrationEndpoint: https://webscraping.ai/oauth/register
    revocationEndpoint: https://webscraping.ai/oauth/revoke
    scopes: {}
    tokenUrl: https://webscraping.ai/oauth/token
    token_endpoint_auth_methods:
    - none
    - client_secret_basic
    - client_secret_post
  name: mcp_oauth2
  sources:
  - well-known/webscraping-ai-oauth-authorization-server.json
  - well-known/webscraping-ai-oauth-protected-resource.json
  type: oauth2
slug: webscraping-ai-authentication
source_filename: webscraping-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: openapi/webscraping-ai-openapi.yml\ndocs: https://webscraping.ai/docs#authentication\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorization_code\nschemes:\n- name: api_key\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: >-\n    All REST API requests require an API key passed as the `api_key` query-string\n    parameter. There is no header form documented. The docs warn the key must not be\n    exposed in client-side code.\n  applies_to: https://api.webscraping.ai\n  sources:\n  - openapi/webscraping-ai-openapi.yml\n  - https://webscraping.ai/docs\n- name: proxy_basic_auth\n  type: http\n  scheme: basic\n  description: >-\n    Proxy Mode (proxy.webscraping.ai:8888) authenticates with HTTP proxy credentials —\n    the username is the API key and the password carries the request parameters\n    (e.g. `js=true&proxy=residential`). The proxy presents a self-signed\
  \ certificate.\n  applies_to: http://proxy.webscraping.ai:8888\n  sources:\n  - https://webscraping.ai/docs\n- name: mcp_oauth2\n  type: oauth2\n  description: >-\n    The hosted remote MCP server (https://mcp.webscraping.ai/mcp) is protected by OAuth 2.1\n    with PKCE and dynamic client registration — no API key is used. Anonymous requests are\n    rejected with 401 and a RFC 9728 `WWW-Authenticate: Bearer resource_metadata=...` challenge.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://webscraping.ai/oauth/authorize\n    tokenUrl: https://webscraping.ai/oauth/token\n    registrationEndpoint: https://webscraping.ai/oauth/register\n    revocationEndpoint: https://webscraping.ai/oauth/revoke\n    code_challenge_methods: [S256]\n    grant_types: [authorization_code, refresh_token]\n    token_endpoint_auth_methods: [none, client_secret_basic, client_secret_post]\n    scopes: {}\n  sources:\n  - well-known/webscraping-ai-oauth-authorization-server.json\n  - well-known/webscraping-ai-oauth-protected-resource.json\n\
  notes:\n- 'The OpenAPI declares a single api_key scheme applied globally — security: [{api_key: []}].'\n- No OAuth scopes are published; the authorization-server metadata omits `scopes_supported`,\n  so no `scopes/` artifact is emitted rather than inventing one.\n- An invalid or missing key returns HTTP 403 (not 401) on the REST API.\nx-evidence:\n- url: https://webscraping.ai/openapi.yml\n  http_status: 200\n- url: https://webscraping.ai/.well-known/oauth-authorization-server\n  http_status: 200\n- url: https://webscraping.ai/.well-known/oauth-protected-resource\n  http_status: 200\n- url: https://mcp.webscraping.ai/mcp\n  http_status: 401\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webscraping-ai/refs/heads/main/authentication/webscraping-ai-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Web Scraping
- Data Extraction
- Proxies
- Artificial Intelligence
- Browser Automation
- Model Context Protocol
- Development
- Public APIs
- ai
- html
- mcp
- llm-tools
- structured-data
- headless-browser
- captcha
---
