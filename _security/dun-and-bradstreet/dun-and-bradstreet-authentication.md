---
api_key_in:
- header
api_specs:
- filename: dun-and-bradstreet-authentication-api-openapi.yml
  format: yaml
  label: Dun & Bradstreet Authentication API
  slug: dun-and-bradstreet-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dun-and-bradstreet/refs/heads/main/openapi/dun-and-bradstreet-authentication-api-openapi.yml
- filename: dun-and-bradstreet-data-file-api-openapi.yml
  format: yaml
  label: Dun & Bradstreet Data File API
  slug: dun-and-bradstreet-data-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dun-and-bradstreet/refs/heads/main/openapi/dun-and-bradstreet-data-file-api-openapi.yml
- filename: dun-and-bradstreet-enrich-api-openapi.yml
  format: yaml
  label: Dun & Bradstreet Enrich API
  slug: dun-and-bradstreet-enrich-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dun-and-bradstreet/refs/heads/main/openapi/dun-and-bradstreet-enrich-api-openapi.yml
- filename: dun-and-bradstreet-identity-resolution-api-openapi.yml
  format: yaml
  label: Dun & Bradstreet Identity Resolution API
  slug: dun-and-bradstreet-identity-resolution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dun-and-bradstreet/refs/heads/main/openapi/dun-and-bradstreet-identity-resolution-api-openapi.yml
- filename: dun-and-bradstreet-monitoring-api-openapi.yml
  format: yaml
  label: Dun & Bradstreet Monitoring API
  slug: dun-and-bradstreet-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dun-and-bradstreet/refs/heads/main/openapi/dun-and-bradstreet-monitoring-api-openapi.yml
- filename: dun-and-bradstreet-multi-process-api-openapi.yml
  format: yaml
  label: Dun & Bradstreet Multi-Process API
  slug: dun-and-bradstreet-multi-process-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dun-and-bradstreet/refs/heads/main/openapi/dun-and-bradstreet-multi-process-api-openapi.yml
- filename: dun-and-bradstreet-research-api-openapi.yml
  format: yaml
  label: Dun & Bradstreet Research API
  slug: dun-and-bradstreet-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dun-and-bradstreet/refs/heads/main/openapi/dun-and-bradstreet-research-api-openapi.yml
- filename: dun-and-bradstreet-search-api-openapi.yml
  format: yaml
  label: Dun & Bradstreet Search API
  slug: dun-and-bradstreet-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dun-and-bradstreet/refs/heads/main/openapi/dun-and-bradstreet-search-api-openapi.yml
auth_types:
- http
- oauth2
- apiKey
description: Dun & Bradstreet runs three distinct authentication models across three surfaces, and they do not share credentials. The Direct+ REST API uses an OAuth 2.0 client_credentials exchange that returns a bearer JWT. The Commercial Graph / Direct+ MCP server uses a single Dplus-API-Key header. The Risk Analytics MCP server runs a full OAuth 2.0 authorization server with PKCE, refresh tokens and scopes. This file supersedes the earlier derived version, which saw only the two http securitySchemes in the spec.
kind: authentication
layout: security
method: searched
name: Dun And Bradstreet Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Dun & Bradstreet secures its APIs with http, oauth2, and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Dun & Bradstreet
provider_slug: dun-and-bradstreet
scheme_count: 4
schemes:
- applies_to: every Direct+ operation except generateAccessToken
  bearerFormat: JWT
  host: https://plus.dnb.com
  in: header
  name: bearerAuth
  note: An anonymous call to a real operation returns HTTP 401 with errorCode "00004" — "You are not currently authorised to access this product. Please contact your D&B account representative". The same 401 covers both a missing token and a valid token without contract entitlement, so an agent cannot distinguish auth failure from entitlement failure from the status code alone.
  obtained_by: POST /v3/token
  parameter: Authorization
  scheme: bearer
  sources:
  - openapi/_original/dnb-direct-plus-openapi-original.yml
  surface: D&B Direct+ REST API
  type: http
- applies_to:
  - generateAccessToken
  credentials: consumer key as username, consumer secret as password
  host: https://plus.dnb.com
  in: header
  name: basicAuth
  note: Used only on POST /v3/token, whose body is {"grant_type":"client_credentials"}. This is an OAuth 2.0 client_credentials grant modelled as an ordinary operation rather than declared as an oauth2 securityScheme, which is why a spec-only reader sees "http basic" instead of OAuth.
  parameter: Authorization
  scheme: basic
  sources:
  - openapi/_original/dnb-direct-plus-openapi-original.yml
  surface: D&B Direct+ token exchange
  type: http
- in: header
  name: Dplus-API-Key
  note: Documented verbatim by the certified Microsoft Power Platform connector as the single required securestring connection parameter. "Dplus" is D&B's shorthand for Direct+.
  parameter: Dplus-API-Key
  sources:
  - https://learn.microsoft.com/en-us/connectors/dunandbradstreetmcps/
  surface: D&B MCP Server (Commercial Graph / Direct+)
  type: apiKey
- challenge: 'An unauthenticated POST to /mcp returns 401 with WWW-Authenticate: Bearer error="invalid_token", error_description="Authentication required.", resource_metadata="https://agents.riskanalytics.dnb.com/.well-known/oauth-protected-resource/mcp"'
  detail: scopes/dun-and-bradstreet-scopes.yml
  discovery:
  - path: /.well-known/oauth-authorization-server
    spec: RFC 8414
    status: 200
  - path: /.well-known/oauth-protected-resource
    spec: RFC 9728
    status: 200
  - path: /.well-known/oauth-protected-resource/mcp
    spec: RFC 9728
    status: 200
  - path: /.well-known/openid-configuration
    status: 404
  flows:
  - authorizationUrl: https://agents.riskanalytics.dnb.com/authorize
    flow: authorizationCode
    scopes:
    - mcp.read
    - mcp.write
    - offline_access
    - openid
    - email
    - profile
    tokenUrl: https://agents.riskanalytics.dnb.com/token
  - flow: clientCredentials
    scopes:
    - mcp.read
    - mcp.write
    tokenUrl: https://agents.riskanalytics.dnb.com/token
  host: https://agents.riskanalytics.dnb.com
  issuer: https://agents.riskanalytics.dnb.com
  name: riskAnalyticsOAuth
  pkce:
  - S256
  - plain
  refresh_tokens: true
  sources:
  - https://agents.riskanalytics.dnb.com/.well-known/oauth-authorization-server
  surface: D&B Risk Analytics remote MCP server
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: dun-and-bradstreet-authentication
source_filename: dun-and-bradstreet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  openapi/_original/dnb-direct-plus-openapi-original.yml +\n  https://agents.riskanalytics.dnb.com/.well-known/oauth-authorization-server +\n  https://learn.microsoft.com/en-us/connectors/dunandbradstreetmcps/ +\n  live probes of https://plus.dnb.com\ndocs: https://directplus.documentation.dnb.com/html/guides/Authentication.html\ndocs_status: 302 (redirects to https://directplus.documentation.dnb.com/oauth2/authorization/okta)\ndescription: >-\n  Dun & Bradstreet runs three distinct authentication models across three\n  surfaces, and they do not share credentials. The Direct+ REST API uses an\n  OAuth 2.0 client_credentials exchange that returns a bearer JWT. The\n  Commercial Graph / Direct+ MCP server uses a single Dplus-API-Key header.\n  The Risk Analytics MCP server runs a full OAuth 2.0 authorization server\n  with PKCE, refresh tokens and scopes. This file supersedes the earlier\n  derived version, which saw only\
  \ the two http securitySchemes in the spec.\n\nsummary:\n  types: [http, oauth2, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials, authorizationCode]\n  http_schemes: [basic, bearer]\n  surfaces: 3\n\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    surface: D&B Direct+ REST API\n    host: https://plus.dnb.com\n    in: header\n    parameter: Authorization\n    sources:\n      - openapi/_original/dnb-direct-plus-openapi-original.yml\n    applies_to: every Direct+ operation except generateAccessToken\n    obtained_by: POST /v3/token\n    note: >-\n      An anonymous call to a real operation returns HTTP 401 with errorCode\n      \"00004\" — \"You are not currently authorised to access this product.\n      Please contact your D&B account representative\". The same 401 covers\n      both a missing token and a valid token without contract entitlement,\n      so an agent cannot distinguish auth failure from entitlement failure\n\
  \      from the status code alone.\n\n  - name: basicAuth\n    type: http\n    scheme: basic\n    surface: D&B Direct+ token exchange\n    host: https://plus.dnb.com\n    in: header\n    parameter: Authorization\n    sources:\n      - openapi/_original/dnb-direct-plus-openapi-original.yml\n    applies_to: [generateAccessToken]\n    credentials: consumer key as username, consumer secret as password\n    note: >-\n      Used only on POST /v3/token, whose body is\n      {\"grant_type\":\"client_credentials\"}. This is an OAuth 2.0\n      client_credentials grant modelled as an ordinary operation rather than\n      declared as an oauth2 securityScheme, which is why a spec-only reader\n      sees \"http basic\" instead of OAuth.\n\n  - name: Dplus-API-Key\n    type: apiKey\n    in: header\n    parameter: Dplus-API-Key\n    surface: D&B MCP Server (Commercial Graph / Direct+)\n    sources:\n      - https://learn.microsoft.com/en-us/connectors/dunandbradstreetmcps/\n    note: >-\n      Documented\
  \ verbatim by the certified Microsoft Power Platform connector\n      as the single required securestring connection parameter. \"Dplus\" is\n      D&B's shorthand for Direct+.\n\n  - name: riskAnalyticsOAuth\n    type: oauth2\n    surface: D&B Risk Analytics remote MCP server\n    host: https://agents.riskanalytics.dnb.com\n    sources:\n      - https://agents.riskanalytics.dnb.com/.well-known/oauth-authorization-server\n    issuer: https://agents.riskanalytics.dnb.com\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://agents.riskanalytics.dnb.com/authorize\n        tokenUrl: https://agents.riskanalytics.dnb.com/token\n        scopes: [mcp.read, mcp.write, offline_access, openid, email, profile]\n      - flow: clientCredentials\n        tokenUrl: https://agents.riskanalytics.dnb.com/token\n        scopes: [mcp.read, mcp.write]\n    pkce: [S256, plain]\n    token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n    refresh_tokens: true\n  \
  \  discovery:\n      - {path: /.well-known/oauth-authorization-server, status: 200, spec: RFC 8414}\n      - {path: /.well-known/oauth-protected-resource, status: 200, spec: RFC 9728}\n      - {path: /.well-known/oauth-protected-resource/mcp, status: 200, spec: RFC 9728}\n      - {path: /.well-known/openid-configuration, status: 404}\n    challenge: >-\n      An unauthenticated POST to /mcp returns 401 with\n      WWW-Authenticate: Bearer error=\"invalid_token\",\n      error_description=\"Authentication required.\",\n      resource_metadata=\"https://agents.riskanalytics.dnb.com/.well-known/oauth-protected-resource/mcp\"\n    detail: scopes/dun-and-bradstreet-scopes.yml\n\ntoken_lifecycle:\n  direct_plus:\n    endpoint: POST https://plus.dnb.com/v3/token\n    grant: client_credentials\n    response_fields: [access_token, token_type, expirationDateTime]\n    expiry_field: expirationDateTime\n    refresh: re-run the client_credentials exchange (no refresh token)\n    revocation_endpoint:\
  \ null\n    introspection_endpoint: null\n  risk_analytics_mcp:\n    refresh: refresh_token grant supported (offline_access scope)\n    revocation_endpoint: null\n    introspection_endpoint: null\n\nonboarding:\n  self_serve: true\n  registration: https://directplus.documentation.dnb.com/registration/register\n  login: https://directplus.documentation.dnb.com/home\n  note: >-\n    Registration is self-serve but the documentation portal behind it, and\n    every credential-provisioning page, sits behind Okta sign-in. API access\n    itself is contract-gated — see plans/dun-and-bradstreet-plans-pricing.yml.\n\nmtls: false\nopenid_connect: false\nopenid_connect_note: >-\n  openid/email/profile appear in the MCP authorization server's\n  scopes_supported, but no OIDC discovery document is served, so D&B is not an\n  OIDC provider by the discovery test.\n\nabsences:\n  - The Direct+ authentication guide is behind the Okta gate.\n  - No token revocation or introspection endpoint on any surface.\n\
  \  - No scope model on the Direct+ REST API — entitlement is contractual.\n  - No mutual TLS option documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dun-and-bradstreet/refs/heads/main/authentication/dun-and-bradstreet-authentication.yml
summary_line: http/oauth2/apiKey · 4 schemes
tags:
- Business Data
- Company Data
- D-U-N-S Number
- Credit
- Risk
- Master Data
- Data Enrichment
- Identity Resolution
- Compliance
- Supply Chain
- Sales Intelligence
- Monitoring
---
