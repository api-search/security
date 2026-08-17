---
api_key_in: []
auth_types: []
description: Highspot runs two distinct authentication surfaces. The REST API (https://api-{instance}.highspot.com/v1.0) uses a static API client key + secret pair issued from Highspot account settings under Developer > Basics — no OAuth, no scopes, no token exchange. The remote MCP server (https://mcp.highspot.com/mcp) uses OAuth 2.1 bearer tokens issued by app.highspot.com, with Dynamic Client Registration, PKCE and refresh tokens. The OAuth half was read from Highspot's own RFC 8414 / RFC 9728 discovery documents; the API-key half is documented only in integrator documentation and in-product settings, because Highspot's developer reference sits behind an authenticated app login.
kind: authentication
layout: security
method: probed
name: Highspot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Highspot declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Highspot
provider_slug: highspot
scheme_count: 3
schemes:
- applies_to: Highspot REST API
  base_url_pattern: https://api-{instance}.highspot.com/{version}
  confidence: medium
  credential_source: Highspot account settings > Developer > Basics. Requires Highspot admin rights to issue.
  evidence:
  - body: Could not authenticate user.
    http_status: 401
    note: Confirms the host is live and the versioned API root is credential-gated.
    url: https://api-su2.highspot.com/v1.0/
  id: highspot-rest-api-key
  note: Recorded from third-party integrator documentation because Highspot publishes no public API reference; developers.highspot.com 302s into the app login.
  observed_instances:
  - https://api-su2.highspot.com/v1.0
  optional_features:
  - description: '"Impersonation in Highspot REST API" can be enabled per API client so requests are evaluated against a named user''s spot-level permissions rather than the API client''s own access.'
    name: Impersonation
    source: https://docs.glean.com/connectors/native/highspot/
  rotation: not documented publicly
  scheme_detail: API client key + API client secret pair
  scopes: none
  sources:
  - https://docs.workato.com/en/connectors/highspot.html
  - https://docs.glean.com/connectors/native/highspot/
  transport: HTTPS
  type: apiKey
  versions_seen:
  - v1.0
  - v0.5
- applies_to: Highspot MCP Server
  bearer_challenge: 'WWW-Authenticate: Bearer realm="mcp-server", resource_metadata="https://mcp.highspot.com/.well-known/oauth-protected-resource/mcp"'
  confidence: high
  dynamic_client_registration:
    registration_endpoint: https://app.highspot.com/auth/oauth2/v1/register
    spec: RFC 7591
    supported: true
  evidence:
  - http_status: 401
    note: JSON-RPC error plus RFC 9728 bearer challenge
    url: https://mcp.highspot.com/mcp
  - http_status: 200
    note: RFC 8414 authorization server metadata
    url: https://app.highspot.com/.well-known/oauth-authorization-server
  - http_status: 200
    note: RFC 9728 protected resource metadata
    url: https://mcp.highspot.com/.well-known/oauth-protected-resource/mcp
  flows:
    authorizationCode:
      authorizationUrl: https://app.highspot.com/oauth2/v1/authorize
      refreshUrl: https://app.highspot.com/auth/oauth2/v1/token
      scopes:
        mcp:read: Read content, answers and analytics through the MCP server
        mcp:write: Create pitches and Digital Rooms and invoke Highspot Agents
        offline_access: Issue a refresh token for unattended agent operation
      tokenUrl: https://app.highspot.com/auth/oauth2/v1/token
  id: highspot-mcp-oauth
  issuer: https://app.highspot.com
  pkce:
    methods_supported:
    - S256
    - plain
    required_by_spec: true
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - none
  type: oauth2
- applies_to: Highspot MCP connector for Microsoft Copilot / Power Platform
  confidence: high
  id: highspot-microsoft-connector
  scheme_detail: Interactive Highspot sign-in from the Copilot for Sales side pane mints the tokens the connector uses. Admins install the connector into the tenant; each user authorizes individually.
  source: https://learn.microsoft.com/en-us/connectors/highspotmcptestjan20/
  type: oauth2
slug: highspot-authentication
source_filename: highspot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Highspot Authentication\ndescription: >-\n  Highspot runs two distinct authentication surfaces. The REST API\n  (https://api-{instance}.highspot.com/v1.0) uses a static API client key + secret\n  pair issued from Highspot account settings under Developer > Basics — no OAuth, no\n  scopes, no token exchange. The remote MCP server (https://mcp.highspot.com/mcp)\n  uses OAuth 2.1 bearer tokens issued by app.highspot.com, with Dynamic Client\n  Registration, PKCE and refresh tokens. The OAuth half was read from Highspot's own\n  RFC 8414 / RFC 9728 discovery documents; the API-key half is documented only in\n  integrator documentation and in-product settings, because Highspot's developer\n  reference sits behind an authenticated app login.\ngenerated: '2026-08-14'\nmethod: probed\nsource: >-\n  https://app.highspot.com/.well-known/oauth-authorization-server +\n  https://mcp.highspot.com/.well-known/oauth-protected-resource/mcp\ndocs: https://www.highspot.com/product/mcp-server/\n\
  checked: '2026-08-14'\n\nschemes:\n  - id: highspot-rest-api-key\n    applies_to: Highspot REST API\n    type: apiKey\n    scheme_detail: API client key + API client secret pair\n    transport: HTTPS\n    credential_source: >-\n      Highspot account settings > Developer > Basics. Requires Highspot admin rights\n      to issue.\n    base_url_pattern: https://api-{instance}.highspot.com/{version}\n    observed_instances:\n      - https://api-su2.highspot.com/v1.0\n    versions_seen:\n      - v1.0\n      - v0.5\n    scopes: none\n    rotation: not documented publicly\n    optional_features:\n      - name: Impersonation\n        description: >-\n          \"Impersonation in Highspot REST API\" can be enabled per API client so\n          requests are evaluated against a named user's spot-level permissions rather\n          than the API client's own access.\n        source: https://docs.glean.com/connectors/native/highspot/\n    evidence:\n      - url: https://api-su2.highspot.com/v1.0/\n \
  \       http_status: 401\n        body: Could not authenticate user.\n        note: >-\n          Confirms the host is live and the versioned API root is credential-gated.\n    sources:\n      - https://docs.workato.com/en/connectors/highspot.html\n      - https://docs.glean.com/connectors/native/highspot/\n    confidence: medium\n    note: >-\n      Recorded from third-party integrator documentation because Highspot publishes no\n      public API reference; developers.highspot.com 302s into the app login.\n\n  - id: highspot-mcp-oauth\n    applies_to: Highspot MCP Server\n    type: oauth2\n    flows:\n      authorizationCode:\n        authorizationUrl: https://app.highspot.com/oauth2/v1/authorize\n        tokenUrl: https://app.highspot.com/auth/oauth2/v1/token\n        refreshUrl: https://app.highspot.com/auth/oauth2/v1/token\n        scopes:\n          mcp:read: Read content, answers and analytics through the MCP server\n          mcp:write: Create pitches and Digital Rooms and invoke\
  \ Highspot Agents\n          offline_access: Issue a refresh token for unattended agent operation\n    issuer: https://app.highspot.com\n    dynamic_client_registration:\n      supported: true\n      registration_endpoint: https://app.highspot.com/auth/oauth2/v1/register\n      spec: RFC 7591\n    pkce:\n      required_by_spec: true\n      methods_supported:\n        - S256\n        - plain\n    token_endpoint_auth_methods_supported:\n      - client_secret_post\n      - none\n    bearer_challenge: >-\n      WWW-Authenticate: Bearer realm=\"mcp-server\",\n      resource_metadata=\"https://mcp.highspot.com/.well-known/oauth-protected-resource/mcp\"\n    evidence:\n      - url: https://mcp.highspot.com/mcp\n        http_status: 401\n        note: JSON-RPC error plus RFC 9728 bearer challenge\n      - url: https://app.highspot.com/.well-known/oauth-authorization-server\n        http_status: 200\n        note: RFC 8414 authorization server metadata\n      - url: https://mcp.highspot.com/.well-known/oauth-protected-resource/mcp\n\
  \        http_status: 200\n        note: RFC 9728 protected resource metadata\n    confidence: high\n\n  - id: highspot-microsoft-connector\n    applies_to: Highspot MCP connector for Microsoft Copilot / Power Platform\n    type: oauth2\n    scheme_detail: >-\n      Interactive Highspot sign-in from the Copilot for Sales side pane mints the\n      tokens the connector uses. Admins install the connector into the tenant; each\n      user authorizes individually.\n    source: https://learn.microsoft.com/en-us/connectors/highspotmcptestjan20/\n    confidence: high\n\nopenid_connect:\n  supported: false\n  evidence:\n    - url: https://app.highspot.com/.well-known/openid-configuration\n      http_status: 200\n      note: >-\n        Answers 200 with the Highspot single-page-app HTML shell, not an OIDC\n        discovery document. Highspot advertises OAuth 2.1 only, with no id_token or\n        openid scope in scopes_supported.\n\nmutual_tls:\n  supported: false\n  note: Not documented on any\
  \ public Highspot surface.\n\ngaps:\n  - >-\n    No public API reference: developers.highspot.com and developer.highspot.com both\n    302 to https://app.highspot.com/unsupported_browser, so the authoritative auth\n    documentation for the REST API is reachable only by licensed customers.\n  - >-\n    No documented key rotation, expiry, or revocation policy for REST API client\n    key/secret pairs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/highspot/refs/heads/main/authentication/highspot-authentication.yml
summary_line: 3 schemes
tags:
- Sales Enablement
- Content Management
- Pitch Analytics
- CRM Integration
- Buyer Engagement
- Training
- Coaching
- AI
- MCP Server
---
