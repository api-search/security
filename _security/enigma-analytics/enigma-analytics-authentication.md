---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Enigma Analytics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Enigma Analytics secures its APIs with apiKey, oauth2, and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Enigma Analytics
provider_slug: enigma-analytics
scheme_count: 4
schemes:
- applies_to:
  - Enigma GraphQL API (https://api.enigma.com/graphql)
  - Enigma KYB REST API (https://api.enigma.com/v2/kyb/)
  - Enigma Screen API (https://api.enigma.com/evaluation/sanctions/screen)
  description: All three developer surfaces require an x-api-key request header carrying an Enigma API key issued from the Enigma Console (https://console.enigma.com). One key, production data, no test-mode variant. Enigma's own Agent Skills note the key contains characters that break shell argument parsing and instruct callers to avoid curl.
  failure:
    body: '{"error_message":"Missing or invalid API key","error_code":"UNAUTHORIZED","retryable":false}'
    http_status: 401
    observed: '2026-08-14'
  in: header
  name: ApiKeyAuth
  parameter_name: x-api-key
  sources:
  - https://documentation.enigma.com/reference/graphql_api/
  - https://www.enigma.com/llms.txt
  type: apiKey
- applies_to: Enigma Screen API (https://api.enigma.com/evaluation/sanctions/screen)
  description: The Screen API takes an additional Account-Name header alongside x-api-key. Enigma's published enigma-screen Agent Skill uses the value `public_evaluation`.
  in: header
  name: AccountNameHeader
  parameter_name: Account-Name
  sources:
  - https://github.com/enigma-io/enigma-claude-plugins
  type: apiKey
- applies_to: Enigma MCP server (https://mcp.enigma.com/mcp)
  description: The remote MCP server implements the MCP OAuth 2.1 authorization profile against https://oauth.enigma.com — authorization_code + refresh_token grants, PKCE S256 required, open dynamic client registration (RFC 7591), token revocation and introspection endpoints, and JWKS served from Amazon Cognito (us-east-1). Authorization-server metadata (RFC 8414) and protected-resource metadata (RFC 9728) are both published and were fetched anonymously.
  failure:
    body: '{"error":"invalid_token","error_description":"Missing or invalid authorization header"}'
    http_status: 401
    observed: '2026-08-14'
  flows:
  - authorizationUrl: https://oauth.enigma.com/authorize
    flow: authorizationCode
    registrationUrl: https://oauth.enigma.com/register
    scopes:
    - openid
    tokenUrl: https://oauth.enigma.com/token
  name: EnigmaMCPOAuth
  see: ../scopes/enigma-analytics-scopes.yml
  sources:
  - https://mcp.enigma.com/.well-known/oauth-authorization-server
  - https://documentation.enigma.com/guides/ai-mcp
  type: oauth2
- applies_to: Enigma MCP server (https://mcp.enigma.com/mcp)
  description: 'Alternative to the OAuth flow: the Console "Agent tools" page emits ready-to-paste MCP client configuration with an Authorization bearer token tied to an Enigma API key pre-filled, for Claude Code, Cursor, VS Code and Gemini CLI.'
  name: BearerAuth
  scheme: bearer
  sources:
  - https://documentation.enigma.com/guides/ai-mcp
  type: http
slug: enigma-analytics-authentication
source_filename: enigma-analytics-authentication.yml
source_heading: Authentication Profile
source_url: https://www.enigma.com/llms.txt
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://www.enigma.com/llms.txt\ndocs: https://documentation.enigma.com/reference/graphql_api/\nsources:\n- https://www.enigma.com/llms.txt\n- https://documentation.enigma.com/reference/graphql_api/\n- https://documentation.enigma.com/guides/ai-mcp\n- https://mcp.enigma.com/.well-known/oauth-authorization-server\n- https://github.com/enigma-io/enigma-claude-plugins\nsummary:\n  types: [apiKey, oauth2, http]\n  api_key_in: [header]\n  api_key_name: x-api-key\n  oauth2_for: MCP server only\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  applies_to:\n  - Enigma GraphQL API (https://api.enigma.com/graphql)\n  - Enigma KYB REST API (https://api.enigma.com/v2/kyb/)\n  - Enigma Screen API (https://api.enigma.com/evaluation/sanctions/screen)\n  description: >-\n    All three developer surfaces require an x-api-key request header carrying an Enigma API key\n    issued from the Enigma Console\
  \ (https://console.enigma.com). One key, production data, no\n    test-mode variant. Enigma's own Agent Skills note the key contains characters that break shell\n    argument parsing and instruct callers to avoid curl.\n  failure:\n    http_status: 401\n    body: '{\"error_message\":\"Missing or invalid API key\",\"error_code\":\"UNAUTHORIZED\",\"retryable\":false}'\n    observed: '2026-08-14'\n  sources:\n  - https://documentation.enigma.com/reference/graphql_api/\n  - https://www.enigma.com/llms.txt\n- name: AccountNameHeader\n  type: apiKey\n  in: header\n  parameter_name: Account-Name\n  applies_to: Enigma Screen API (https://api.enigma.com/evaluation/sanctions/screen)\n  description: >-\n    The Screen API takes an additional Account-Name header alongside x-api-key. Enigma's published\n    enigma-screen Agent Skill uses the value `public_evaluation`.\n  sources:\n  - https://github.com/enigma-io/enigma-claude-plugins\n- name: EnigmaMCPOAuth\n  type: oauth2\n  applies_to: Enigma MCP\
  \ server (https://mcp.enigma.com/mcp)\n  description: >-\n    The remote MCP server implements the MCP OAuth 2.1 authorization profile against\n    https://oauth.enigma.com — authorization_code + refresh_token grants, PKCE S256 required, open\n    dynamic client registration (RFC 7591), token revocation and introspection endpoints, and JWKS\n    served from Amazon Cognito (us-east-1). Authorization-server metadata (RFC 8414) and\n    protected-resource metadata (RFC 9728) are both published and were fetched anonymously.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.enigma.com/authorize\n    tokenUrl: https://oauth.enigma.com/token\n    registrationUrl: https://oauth.enigma.com/register\n    scopes: [openid]\n  failure:\n    http_status: 401\n    body: '{\"error\":\"invalid_token\",\"error_description\":\"Missing or invalid authorization header\"}'\n    observed: '2026-08-14'\n  see: ../scopes/enigma-analytics-scopes.yml\n  sources:\n  - https://mcp.enigma.com/.well-known/oauth-authorization-server\n\
  \  - https://documentation.enigma.com/guides/ai-mcp\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  applies_to: Enigma MCP server (https://mcp.enigma.com/mcp)\n  description: >-\n    Alternative to the OAuth flow: the Console \"Agent tools\" page emits ready-to-paste MCP client\n    configuration with an Authorization bearer token tied to an Enigma API key pre-filled, for Claude\n    Code, Cursor, VS Code and Gemini CLI.\n  sources:\n  - https://documentation.enigma.com/guides/ai-mcp\nsso:\n  console: https://documentation.enigma.com/console/sso-configuration\n  note: The Console supports customer SSO configuration; this governs human Console access, not API calls.\ngaps:\n- No OpenID Connect discovery document is served on any host, though `openid` is the only advertised OAuth scope.\n- No per-scope authorization on the MCP surface — an authorized client gets the whole tool set.\n- No key rotation, expiry or IP-allowlist policy is published for x-api-key.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enigma-analytics/refs/heads/main/authentication/enigma-analytics-authentication.yml
summary_line: apiKey/oauth2/http · 4 schemes
tags:
- Company
- Business Data
- KYB
- Identity Verification
- Compliance
- Sanctions Screening
- GraphQL
- Fintech
- Data Enrichment
- MCP
- Agent Skills
- Payments Risk
---
