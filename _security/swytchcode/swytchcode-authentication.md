---
anonymous_access: false
api_key_in: []
auth_types: []
description: Two separate authentication planes. No hosted public API — auth applies to the CLI / MCP server / Runtime SDKs.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Swytchcode Authentication
name_suffix: Authentication
oauth_flows: []
overview: Swytchcode declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Swytchcode
provider_slug: swytchcode
scheme_count: 3
schemes:
- description: Swytchcode account identity via `swy login` browser device flow; session stored at ~/.swytchcode/auth.json.
  flow: device
  name: account-oauth-device-flow
  type: oauth2
- description: Service-token auth for CI/servers; read from process environment only (deliberately never from .env files).
  in: environment
  key: SWYTCHCODE_TOKEN
  name: account-service-token
  type: apiKey
- description: The optional local HTTP/SSE MCP transport requires a bearer token stored at ~/.swytchcode/mcp_token (`swy mcp token`). stdio transport needs no auth.
  name: mcp-http-bearer
  scheme: bearer
  type: http
slug: swytchcode-authentication
source_filename: swytchcode-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\nsource: https://docs.swytchcode.com/guides/authentication/ , https://docs.swytchcode.com/guides/managed-authentication/ , https://docs.swytchcode.com/cli/authentication/\ndocs: https://docs.swytchcode.com/guides/authentication/\ndescription: >-\n  Two separate authentication planes. No hosted public API — auth applies to the CLI / MCP\n  server / Runtime SDKs.\nschemes:\n  - name: account-oauth-device-flow\n    type: oauth2\n    flow: device\n    description: Swytchcode account identity via `swy login` browser device flow; session stored at ~/.swytchcode/auth.json.\n  - name: account-service-token\n    type: apiKey\n    in: environment\n    key: SWYTCHCODE_TOKEN\n    description: Service-token auth for CI/servers; read from process environment only (deliberately never from .env files).\n  - name: mcp-http-bearer\n    type: http\n    scheme: bearer\n    description: The optional local HTTP/SSE MCP transport requires a bearer token stored\
  \ at ~/.swytchcode/mcp_token (`swy mcp token`). stdio transport needs no auth.\nprovider_credentials:\n  description: >-\n    Third-party provider credentials (OAuth, API keys, bearer tokens) are resolved separately\n    from account auth, in priority order: environment variables, the encrypted managed\n    credential store (WorkOS-managed auth), then the project .env file. Managed via\n    `swy auth connect/status/disconnect`. Account credentials are never used against external\n    providers.\n  managed_by: WorkOS\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swytchcode/refs/heads/main/authentication/swytchcode-authentication.yml
summary_line: 3 schemes
tags:
- AI / Agent Tooling
- agentic middleware
- API Integration
- API Orchestration
- API execution layer
- LLM tool execution
- MCP Server
- Developer Tools
- API Documentation
- API playground
---
