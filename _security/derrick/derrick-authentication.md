---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Derrick Authentication
name_suffix: Authentication
oauth_flows: []
overview: Derrick declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Derrick
provider_slug: derrick
scheme_count: 3
schemes:
- description: The derrick-mcp package sends the API key as an X-API-Key header on every https://app1.derrick-app.com/api/v1/* call. Anonymous requests return 401 {"success":false,"error":"Invalid or missing API key","errorType":"AUTH"} (probed 2026-09-09).
  header: X-API-Key
  in: header
  name: api_key_header
  surfaces:
  - REST API
  type: apiKey
- description: 'The MCP server card documents Authorization: Bearer <api-key> on https://app1.derrick-app.com/mcp; required_at_install is false - the server prompts for a key on the first tool call.'
  name: bearer_api_key
  scheme: bearer
  surfaces:
  - MCP remote endpoint
  type: http
- description: RFC 8414 authorization-server metadata served at /.well-known/oauth-authorization-server (probed 200, 2026-09-09); grants authorization_code + refresh_token, token_endpoint_auth client_secret_post or none, PKCE S256 only. The MCP endpoint's WWW-Authenticate challenge points at RFC 9728 resource metadata /.well-known/oauth-protected-resource/mcp. No scopes are published (scopes are not defined in the metadata and no scopes reference page exists).
  dynamic_client_registration: https://app1.derrick-app.com/register
  flows:
    authorizationCode:
      authorizationUrl: https://app1.derrick-app.com/authorize
      refreshUrl: https://app1.derrick-app.com/token
      scopes: {}
      tokenUrl: https://app1.derrick-app.com/token
  name: oauth2_authorization_code
  pkce: S256
  revocation: https://app1.derrick-app.com/revoke
  surfaces:
  - MCP remote endpoint
  type: oauth2
slug: derrick-authentication
source_filename: derrick-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: searched\nsource: >-\n  npm derrick-mcp@0.3.0 (dist/api.js, dist/config.js) + https://app1.derrick-app.com/.well-known/oauth-authorization-server\n  + https://app1.derrick-app.com/.well-known/oauth-protected-resource/mcp + live 401 probes of\n  https://app1.derrick-app.com/api/v1/openapi.json and https://app1.derrick-app.com/mcp\nnote: >-\n  No OpenAPI securitySchemes exist (no OpenAPI is published); this profile is read from the\n  provider's own npm client code, its RFC 8414/9728 discovery documents, and live unauthenticated\n  probes. API keys are issued in the Google Sheets add-on (Derrick menu > API) and require a paid\n  plan (see plans artifact for the Standard-vs-Plus gate discrepancy).\nschemes:\n  - name: api_key_header\n    type: apiKey\n    in: header\n    header: X-API-Key\n    surfaces: [REST API]\n    description: >-\n      The derrick-mcp package sends the API key as an X-API-Key header on every\n      https://app1.derrick-app.com/api/v1/*\
  \ call. Anonymous requests return\n      401 {\"success\":false,\"error\":\"Invalid or missing API key\",\"errorType\":\"AUTH\"} (probed 2026-09-09).\n  - name: bearer_api_key\n    type: http\n    scheme: bearer\n    surfaces: [MCP remote endpoint]\n    description: >-\n      The MCP server card documents Authorization: Bearer <api-key> on https://app1.derrick-app.com/mcp;\n      required_at_install is false - the server prompts for a key on the first tool call.\n  - name: oauth2_authorization_code\n    type: oauth2\n    surfaces: [MCP remote endpoint]\n    flows:\n      authorizationCode:\n        authorizationUrl: https://app1.derrick-app.com/authorize\n        tokenUrl: https://app1.derrick-app.com/token\n        refreshUrl: https://app1.derrick-app.com/token\n        scopes: {}\n    pkce: S256\n    dynamic_client_registration: https://app1.derrick-app.com/register\n    revocation: https://app1.derrick-app.com/revoke\n    description: >-\n      RFC 8414 authorization-server metadata\
  \ served at\n      /.well-known/oauth-authorization-server (probed 200, 2026-09-09); grants authorization_code +\n      refresh_token, token_endpoint_auth client_secret_post or none, PKCE S256 only. The MCP endpoint's\n      WWW-Authenticate challenge points at RFC 9728 resource metadata\n      /.well-known/oauth-protected-resource/mcp. No scopes are published (scopes are not defined in\n      the metadata and no scopes reference page exists).\nenvironment_keys:\n  - DERRICK_API_KEY\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/derrick/refs/heads/main/authentication/derrick-authentication.yml
summary_line: 3 schemes
tags:
- b2b-data-enrichment
- email-finder
- phone-finder
- company-firmographics
- lead-generation
- sales-intelligence
- crm-enrichment
- tech-stack-detection
- email-verification
- siret-siren-france
- mcp-server
- llms-txt
- google-sheets
- gtm-tools
---
