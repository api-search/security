---
api_key_in:
- config-file
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Kotzilla Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Kotzilla secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Kotzilla
provider_slug: kotzilla
scheme_count: 2
schemes:
- bearer_methods_supported:
  - header
  code_challenge_methods_supported:
  - S256
  description: OAuth 2.0 authorization-code flow with PKCE protecting the Kotzilla MCP Server. Advertised anonymously at https://mcp.kotzilla.io/.well-known/oauth-authorization-server. The MCP server is both the resource server and its own authorization server.
  flows:
  - authorizationUrl: https://mcp.kotzilla.io/oauth/authorize
    flow: authorizationCode
    registrationUrl: https://mcp.kotzilla.io/oauth/register
    revocationUrl: https://mcp.kotzilla.io/oauth/revoke
    scopes:
      email: Email address of the authenticated Kotzilla account
      offline_access: Issue a refresh token for long-lived agent sessions
      openid: OpenID Connect subject identifier for the Kotzilla account
    tokenUrl: https://mcp.kotzilla.io/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  name: KotzillaMCPOAuth
  observations:
  - '`token_endpoint_auth_methods_supported: ["none"]` plus a public registration_endpoint means clients are PUBLIC clients registered dynamically (RFC 7591) and authenticated by PKCE alone — the correct and expected posture for an MCP server serving arbitrary agent clients.'
  - An unauthenticated POST of tools/list to https://mcp.kotzilla.io/mcp returns HTTP 401 with {"error":"invalid_token","error_description":"The access token is missing or invalid"} — the resource server enforces the token.
  - '`openid` is offered as a scope but no /.well-known/openid-configuration is served on mcp.kotzilla.io (404), so this is OAuth 2.0 with an OIDC-style scope name rather than a full OIDC provider.'
  response_types_supported:
  - code
  sources:
  - well-known/kotzilla-oauth-authorization-server.json
  - well-known/kotzilla-oauth-protected-resource.json
  surface: https://mcp.kotzilla.io/mcp
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
- description: The Kotzilla SDK authenticates to the platform with a per-application API key delivered in the `kotzilla.json` project file generated from the Console (or by the MCP `generate_app_config` tool). The SDK docs state transmission uses "HTTPS encryption" with "authentication tokens and API Keys". The ingestion hostname is not published in the documentation and no api.kotzilla.io host resolves, so the ingest endpoint is NOT recorded here rather than guessed.
  in: config-file
  name: KotzillaSDKApiKey
  name_hint: kotzilla.json
  sources:
  - https://doc.kotzilla.io/docs/settings/projectFile
  - https://doc.kotzilla.io/docs/discover/sdkData
  surface: Kotzilla SDK -> Kotzilla Platform telemetry ingestion
  type: apiKey
slug: kotzilla-authentication
source_filename: kotzilla-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nsource: https://mcp.kotzilla.io/.well-known/oauth-authorization-server\ndocs:\n  - https://doc.kotzilla.io/docs/getstartedCustom/mcpSetup\n  - https://doc.kotzilla.io/docs/getstartedCustom/consoleSetup\n  - https://doc.kotzilla.io/docs/settings/projectFile\nnote: >-\n  Authored from the provider's own RFC 8414 / RFC 9728 metadata documents and\n  setup docs, NOT derived from an OpenAPI — Kotzilla publishes no OpenAPI\n  (see mcp/kotzilla-mcp.yml). Kotzilla runs two distinct authentication\n  surfaces: OAuth 2.1 on the MCP server for agents/humans, and an API-key model\n  for SDK telemetry ingestion from the instrumented app.\n\nsummary:\n  types: [oauth2, apiKey]\n  api_key_in: [config-file]\n  oauth2_flows: [authorizationCode]\n  pkce_required: true\n  dynamic_client_registration: true\n\nschemes:\n  - name: KotzillaMCPOAuth\n    type: oauth2\n    surface: https://mcp.kotzilla.io/mcp\n    description: >-\n      OAuth 2.0 authorization-code\
  \ flow with PKCE protecting the Kotzilla MCP\n      Server. Advertised anonymously at\n      https://mcp.kotzilla.io/.well-known/oauth-authorization-server. The MCP\n      server is both the resource server and its own authorization server.\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcp.kotzilla.io/oauth/authorize\n        tokenUrl: https://mcp.kotzilla.io/oauth/token\n        registrationUrl: https://mcp.kotzilla.io/oauth/register\n        revocationUrl: https://mcp.kotzilla.io/oauth/revoke\n        scopes:\n          openid: OpenID Connect subject identifier for the Kotzilla account\n          email: Email address of the authenticated Kotzilla account\n          offline_access: Issue a refresh token for long-lived agent sessions\n    grant_types_supported: [authorization_code, refresh_token]\n    response_types_supported: [code]\n    code_challenge_methods_supported: [S256]\n    token_endpoint_auth_methods_supported: [none]\n    bearer_methods_supported:\
  \ [header]\n    sources:\n      - well-known/kotzilla-oauth-authorization-server.json\n      - well-known/kotzilla-oauth-protected-resource.json\n    observations:\n      - >-\n        `token_endpoint_auth_methods_supported: [\"none\"]` plus a public\n        registration_endpoint means clients are PUBLIC clients registered\n        dynamically (RFC 7591) and authenticated by PKCE alone — the correct\n        and expected posture for an MCP server serving arbitrary agent clients.\n      - >-\n        An unauthenticated POST of tools/list to https://mcp.kotzilla.io/mcp\n        returns HTTP 401 with\n        {\"error\":\"invalid_token\",\"error_description\":\"The access token is\n        missing or invalid\"} — the resource server enforces the token.\n      - >-\n        `openid` is offered as a scope but no /.well-known/openid-configuration\n        is served on mcp.kotzilla.io (404), so this is OAuth 2.0 with an\n        OIDC-style scope name rather than a full OIDC provider.\n\n  -\
  \ name: KotzillaSDKApiKey\n    type: apiKey\n    in: config-file\n    name_hint: kotzilla.json\n    surface: Kotzilla SDK -> Kotzilla Platform telemetry ingestion\n    description: >-\n      The Kotzilla SDK authenticates to the platform with a per-application API\n      key delivered in the `kotzilla.json` project file generated from the\n      Console (or by the MCP `generate_app_config` tool). The SDK docs state\n      transmission uses \"HTTPS encryption\" with \"authentication tokens and API\n      Keys\". The ingestion hostname is not published in the documentation and\n      no api.kotzilla.io host resolves, so the ingest endpoint is NOT recorded\n      here rather than guessed.\n    sources:\n      - https://doc.kotzilla.io/docs/settings/projectFile\n      - https://doc.kotzilla.io/docs/discover/sdkData\n\naccount:\n  signup: https://console.kotzilla.io/signup\n  console: https://console.kotzilla.io/\n  note: A free Kotzilla account is the credential root for both surfaces.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kotzilla/refs/heads/main/authentication/kotzilla-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Company
- Ai Data
- Observability
- Monitoring
- Developer Tools
- Kotlin
- Android
- Mobile
- Dependency Injection
- Performance
- MCP
- Agents
---
