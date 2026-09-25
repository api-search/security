---
anonymous_access: false
api_key_in: []
api_specs:
- filename: patronus-protect-openapi.json
  format: json
  label: Patronus Scan API
  slug: patronus-scan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/patronus-protect/refs/heads/main/openapi/patronus-protect-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Patronus Protect Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Patronus Protect secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Patronus Protect
provider_slug: patronus-protect
scheme_count: 2
schemes:
- applies_to: REST Scan API (control.patronus.studio/api/v1) and API-key MCP access
  description: Server-to-server access to the Scan API uses a bearer API key in the Authorization header. The SDK reads it from the PATRONUS_API_KEY environment variable. A rate-limited anonymous allowance exists for public-URL scans without a key; MCP-server audits always require an authenticated key.
  format: Bearer <PATRONUS_API_KEY>
  in: header
  name: apiKey
  parameter_name: Authorization
  scheme: bearer
  sources:
  - sdk/python/client.py
  type: http
- applies_to: Remote MCP server (control.patronus.studio/api/mcp)
  description: The remote MCP server is protected by OAuth 2.1 (authorization code + PKCE, public clients via Dynamic Client Registration). Handled by the MCP host, not the API-key SDK clients.
  flows:
  - authorization_endpoint: https://control.patronus.studio/mcp-authorize
    authorization_server: https://control.patronus.studio
    bearer_methods:
    - header
    flow: authorizationCode
    grant_types:
    - authorization_code
    pkce: S256
    registration_endpoint: https://control.patronus.studio/api/oauth/mcp/register
    resource: https://control.patronus.studio/api
    scopes:
    - scan:read
    - scan:write
    token_endpoint: https://control.patronus.studio/api/oauth/mcp/token
    token_endpoint_auth_methods:
    - none
  name: oauth2
  sources:
  - well-known/patronus-protect-oauth-authorization-server.json
  - well-known/patronus-protect-oauth-protected-resource.json
  type: oauth2
slug: patronus-protect-authentication
source_filename: patronus-protect-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-20'\nmethod: derived\nsource: >-\n  API-key scheme derived from the provider's first-party SDK client\n  (github.com/patronus-protect/patronus-security-cli sdk/python/src/patronus_api_client/client.py).\n  OAuth2 scheme from live discovery at control.patronus.studio/.well-known/oauth-authorization-server\n  and /.well-known/oauth-protected-resource plus the 401 challenge on control.patronus.studio/api/mcp.\n  The authoritative OpenAPI (docs.patronus.studio/openapi.json) is Cloudflare JS-challenged and was\n  not fetchable, so the API-key scheme is derived from the SDK rather than the spec securitySchemes.\nsummary:\n  types: [http, oauth2]\n  http_bearer: true\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  in: header\n  parameter_name: Authorization\n  format: \"Bearer <PATRONUS_API_KEY>\"\n  applies_to: REST Scan API (control.patronus.studio/api/v1) and API-key MCP access\n  description: >-\n    Server-to-server\
  \ access to the Scan API uses a bearer API key in the Authorization header. The\n    SDK reads it from the PATRONUS_API_KEY environment variable. A rate-limited anonymous allowance\n    exists for public-URL scans without a key; MCP-server audits always require an authenticated key.\n  sources: [sdk/python/client.py]\n- name: oauth2\n  type: oauth2\n  applies_to: Remote MCP server (control.patronus.studio/api/mcp)\n  description: >-\n    The remote MCP server is protected by OAuth 2.1 (authorization code + PKCE, public clients via\n    Dynamic Client Registration). Handled by the MCP host, not the API-key SDK clients.\n  flows:\n  - flow: authorizationCode\n    resource: https://control.patronus.studio/api\n    authorization_server: https://control.patronus.studio\n    authorization_endpoint: https://control.patronus.studio/mcp-authorize\n    token_endpoint: https://control.patronus.studio/api/oauth/mcp/token\n    registration_endpoint: https://control.patronus.studio/api/oauth/mcp/register\n\
  \    pkce: S256\n    grant_types: [authorization_code]\n    token_endpoint_auth_methods: [none]\n    scopes: [scan:read, scan:write]\n    bearer_methods: [header]\n  sources:\n  - well-known/patronus-protect-oauth-authorization-server.json\n  - well-known/patronus-protect-oauth-protected-resource.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/patronus-protect/refs/heads/main/authentication/patronus-protect-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- AI Safety
- Prompt Injection
- Security
- LLM
- Agent-Native
- MCP
- DLP
- PII
- On-Device
- AI Firewall
---
