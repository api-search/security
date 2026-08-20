---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Conviva Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Conviva secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Conviva
provider_slug: conviva
scheme_count: 3
schemes:
- applies_to:
  - Conviva Metrics V3 API
  - Conviva Sessions V3 API
  - Conviva AI Alerts API
  - Conviva Bulk Filters API
  - Conviva Precision Policy API
  - Conviva PII Opt-Out API
  - Conviva Validation Timeline API v2
  credential:
    encoding: echo -n "{client_id}:{client_secret}" | base64
    fields:
    - client-Id
    - client-secret
    header: 'Authorization: Basic {base64(client_id:client_secret)}'
    issued_at: Pulse -> API Management page
    kind: api key pair
  errors:
    insufficient_privilege: 403 Forbidden — API not activated for the c3 account, or no edit permission
    invalid_credentials: 401 Unauthorized — Invalid HTTP Authorization / check the credentials
  name: convivaApiKeyBasic
  scheme: basic
  scoping:
    note: Credentials, rate limits and data access are all scoped to a c3 account.
    unit: c3 account
  type: http
  warnings:
  - '"Do not use Pulse user-based credentials for any API request. Pulse user-based credentials and Conviva API keys are different. Calling any Conviva APIs with Pulse user-based credentials results in unrecognized credentials and authentication failure."'
  - Precision Policy POST operations require credentials created by a Precision Admin; otherwise the API returns HTTP 403 Forbidden.
- applies_to:
  - Conviva MCP Server (https://mcp.conviva.com/mcp)
  - Conviva DPI MCP Server (https://dpi-mcp.conviva.com/mcp)
  challenge_observed: 'WWW-Authenticate: Bearer realm="mcp", error="invalid_request", error_description="Missing or malformed Authorization header"'
  discovery:
    authorization_server_metadata: RFC 8414 (/.well-known/oauth-authorization-server) — 200 on both hosts
    dynamic_client_registration: RFC 7591 (/oauth/register advertised on both hosts)
    protected_resource_metadata: RFC 9728 (/.well-known/oauth-protected-resource) — 200 on both hosts
  flows:
  - authorizationUrl: https://mcp.conviva.com/oauth/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    jwksUri: https://mcp.conviva.com/.well-known/jwks.json
    pkce: S256
    registrationUrl: https://mcp.conviva.com/oauth/register
    scopes:
    - openid
    - profile
    - email
    - conviva
    server: https://mcp.conviva.com
    tokenUrl: https://mcp.conviva.com/oauth/token
    token_endpoint_auth_methods:
    - none
  - authorizationUrl: https://dpi-mcp.conviva.com/oauth/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    identity_provider: Okta
    jwksUri: https://dpi-mcp.conviva.com/.well-known/jwks.json
    pkce: S256
    registrationUrl: https://dpi-mcp.conviva.com/oauth/register
    scopes:
    - openid
    - profile
    - email
    - conviva
    server: https://dpi-mcp.conviva.com
    tokenUrl: https://dpi-mcp.conviva.com/oauth/token
    token_endpoint_auth_methods:
    - none
  name: convivaMcpOAuth
  type: oauth2
- applies_to:
  - Conviva MCP Server (https://mcp.conviva.com/mcp)
  credential:
    fields:
    - client_id
    - client_secret
    header: 'Authorization: Basic <base64(client_id:client_secret)>'
    issued_at: Pulse -> API Management page
    kind: api key pair
  name: convivaMcpBasic
  note: Docs recommend OAuth over Basic for MCP because OAuth carries user-based authorization and scopes access to the c3 accounts the user is entitled to.
  purpose: Non-interactive / autonomous agent access where a browser OAuth round-trip is impossible.
  scheme: basic
  type: http
slug: conviva-authentication
source_filename: conviva-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: https://docs.conviva.ai/connect-data/apis/\ndocs:\n- https://docs.conviva.ai/connect-data/apis/\n- https://docs.conviva.ai/vsi-pages/api-mgt/api-management-4129047/\n- https://docs.conviva.ai/connect-data/mcp/\n- https://mcp.conviva.com/.well-known/oauth-authorization-server\n- https://dpi-mcp.conviva.com/.well-known/oauth-authorization-server\nnote: >-\n  Derived by SEARCH of the docs, not from OpenAPI — Conviva publishes no machine-readable spec\n  (its own APIs page says the Scalar/OpenAPI references \"are being wired up separately\"), so\n  there are no securitySchemes objects to aggregate.\n\nsummary:\n  types: [http, oauth2]\n  http_schemes: [basic]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  surfaces:\n    rest: 'HTTP Basic with a Conviva API key pair (client-id : client-secret)'\n    mcp: OAuth 2.1 authorization_code + PKCE S256 with dynamic client registration; HTTP Basic\n      accepted on mcp.conviva.com\
  \ for autonomous agents\n\nschemes:\n- name: convivaApiKeyBasic\n  type: http\n  scheme: basic\n  applies_to:\n  - Conviva Metrics V3 API\n  - Conviva Sessions V3 API\n  - Conviva AI Alerts API\n  - Conviva Bulk Filters API\n  - Conviva Precision Policy API\n  - Conviva PII Opt-Out API\n  - Conviva Validation Timeline API v2\n  credential:\n    kind: api key pair\n    fields: [client-Id, client-secret]\n    issued_at: Pulse -> API Management page\n    encoding: 'echo -n \"{client_id}:{client_secret}\" | base64'\n    header: 'Authorization: Basic {base64(client_id:client_secret)}'\n  warnings:\n  - >-\n    \"Do not use Pulse user-based credentials for any API request. Pulse user-based credentials and\n    Conviva API keys are different. Calling any Conviva APIs with Pulse user-based credentials\n    results in unrecognized credentials and authentication failure.\"\n  - Precision Policy POST operations require credentials created by a Precision Admin; otherwise\n    the API returns HTTP\
  \ 403 Forbidden.\n  errors:\n    invalid_credentials: 401 Unauthorized — Invalid HTTP Authorization / check the credentials\n    insufficient_privilege: 403 Forbidden — API not activated for the c3 account, or no edit permission\n  scoping:\n    unit: c3 account\n    note: Credentials, rate limits and data access are all scoped to a c3 account.\n\n- name: convivaMcpOAuth\n  type: oauth2\n  applies_to:\n  - Conviva MCP Server (https://mcp.conviva.com/mcp)\n  - Conviva DPI MCP Server (https://dpi-mcp.conviva.com/mcp)\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.conviva.com/oauth/authorize\n    tokenUrl: https://mcp.conviva.com/oauth/token\n    registrationUrl: https://mcp.conviva.com/oauth/register\n    jwksUri: https://mcp.conviva.com/.well-known/jwks.json\n    scopes: [openid, profile, email, conviva]\n    pkce: S256\n    token_endpoint_auth_methods: [none]\n    grant_types: [authorization_code, refresh_token]\n    server: https://mcp.conviva.com\n  - flow:\
  \ authorizationCode\n    authorizationUrl: https://dpi-mcp.conviva.com/oauth/authorize\n    tokenUrl: https://dpi-mcp.conviva.com/oauth/token\n    registrationUrl: https://dpi-mcp.conviva.com/oauth/register\n    jwksUri: https://dpi-mcp.conviva.com/.well-known/jwks.json\n    scopes: [openid, profile, email, conviva]\n    pkce: S256\n    token_endpoint_auth_methods: [none]\n    grant_types: [authorization_code, refresh_token]\n    server: https://dpi-mcp.conviva.com\n    identity_provider: Okta\n  discovery:\n    authorization_server_metadata: RFC 8414 (/.well-known/oauth-authorization-server) — 200 on both hosts\n    protected_resource_metadata: RFC 9728 (/.well-known/oauth-protected-resource) — 200 on both hosts\n    dynamic_client_registration: RFC 7591 (/oauth/register advertised on both hosts)\n  challenge_observed: 'WWW-Authenticate: Bearer realm=\"mcp\", error=\"invalid_request\",\n    error_description=\"Missing or malformed Authorization header\"'\n\n- name: convivaMcpBasic\n \
  \ type: http\n  scheme: basic\n  applies_to:\n  - Conviva MCP Server (https://mcp.conviva.com/mcp)\n  credential:\n    kind: api key pair\n    fields: [client_id, client_secret]\n    issued_at: Pulse -> API Management page\n    header: 'Authorization: Basic <base64(client_id:client_secret)>'\n  purpose: Non-interactive / autonomous agent access where a browser OAuth round-trip is impossible.\n  note: >-\n    Docs recommend OAuth over Basic for MCP because OAuth carries user-based authorization and\n    scopes access to the c3 accounts the user is entitled to.\n\nsso:\n  customer_sso: https://docs.conviva.ai/conviva-overview/conviva-sso-federation/\n  note: Conviva Pulse supports SSO federation for portal users — separate from API credentials.\n\ngaps:\n- No OpenID Connect discovery document (/.well-known/openid-configuration) on any Conviva host.\n- No API-key-in-header or query-parameter scheme; Basic only on the REST surface.\n- No mutualTLS.\n- No machine-readable securitySchemes because\
  \ no OpenAPI is published.\n\nx-evidence:\n  fetched: '2026-08-01'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conviva/refs/heads/main/authentication/conviva-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Analytics
- Streaming
- Video
- Observability
- Monitoring
- Media
- Quality of Experience
- Real-Time
- Telemetry
- Agents
- MCP
- Company
---
