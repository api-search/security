---
api_key_in:
- header
api_specs:
- filename: harmonic-ai-companies-api-openapi.yml
  format: yaml
  label: Harmonic REST & GraphQL API
  slug: harmonic-rest-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harmonic-ai/refs/heads/main/openapi/harmonic-ai-companies-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Harmonic Ai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Harmonic.ai secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Harmonic.ai
provider_slug: harmonic-ai
scheme_count: 2
schemes:
- description: Include your Harmonic API key as the `apikey` header on requests to api.harmonic.ai. Obtain the key from your Harmonic account settings (console.harmonic.ai). Recommended for programmatic / server-to-server access, including API-key auth to the MCP server.
  in: header
  name: apiKey
  parameter_name: apikey
  sources:
  - llms.txt
  type: apiKey
- description: OAuth 2.0 used by the MCP server and web application; authenticates through console.harmonic.ai with Firebase JWT tokens and supports automatic token refresh.
  flows:
  - authorization_endpoint: https://mcp.api.harmonic.ai/authorize
    authorization_server: https://mcp.api.harmonic.ai/
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce: S256
    registration_endpoint: https://mcp.api.harmonic.ai/register
    scopes:
    - read
    - write
    token_endpoint: https://mcp.api.harmonic.ai/token
  name: oauth2
  sources:
  - well-known/harmonic-ai-mcp-oauth-authorization-server.json
  - llms.txt
  type: oauth2
slug: harmonic-ai-authentication
source_filename: harmonic-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://console.harmonic.ai/ (llms.txt \"API Authentication\") + https://mcp.api.harmonic.ai/.well-known/oauth-authorization-server\ndocs: https://console.harmonic.ai/docs/api-reference/introduction\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n  - name: apiKey\n    type: apiKey\n    in: header\n    parameter_name: apikey\n    description: >-\n      Include your Harmonic API key as the `apikey` header on requests to api.harmonic.ai.\n      Obtain the key from your Harmonic account settings (console.harmonic.ai). Recommended for\n      programmatic / server-to-server access, including API-key auth to the MCP server.\n    sources: [llms.txt]\n  - name: oauth2\n    type: oauth2\n    description: >-\n      OAuth 2.0 used by the MCP server and web application; authenticates through console.harmonic.ai\n      with Firebase JWT tokens and supports automatic token refresh.\n\
  \    flows:\n      - flow: authorizationCode\n        authorization_server: https://mcp.api.harmonic.ai/\n        authorization_endpoint: https://mcp.api.harmonic.ai/authorize\n        token_endpoint: https://mcp.api.harmonic.ai/token\n        registration_endpoint: https://mcp.api.harmonic.ai/register\n        pkce: S256\n        grant_types: [authorization_code, refresh_token]\n        scopes: [read, write]\n    sources: [well-known/harmonic-ai-mcp-oauth-authorization-server.json, llms.txt]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harmonic-ai/refs/heads/main/authentication/harmonic-ai-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- startup-intelligence
- venture-capital
- company-data
- people-data
- investor-data
- funding-data
- Data Enrichment
- sales-intelligence
- Market Intelligence
- graphql
- MCP
- agent-native
---
