---
api_key_in:
- header
api_specs:
- filename: leadspace-authorization-api-openapi.yml
  format: yaml
  label: Leadspace Authorization API
  slug: leadspace-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadspace/refs/heads/main/openapi/leadspace-authorization-api-openapi.yml
- filename: leadspace-discovery-api-openapi.yml
  format: yaml
  label: Leadspace Discovery API
  slug: leadspace-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadspace/refs/heads/main/openapi/leadspace-discovery-api-openapi.yml
- filename: leadspace-enrichment-api-openapi.yml
  format: yaml
  label: Leadspace Enrichment API
  slug: leadspace-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadspace/refs/heads/main/openapi/leadspace-enrichment-api-openapi.yml
- filename: leadspace-intent-api-openapi.yml
  format: yaml
  label: Leadspace Intent API
  slug: leadspace-intent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadspace/refs/heads/main/openapi/leadspace-intent-api-openapi.yml
- filename: leadspace-results-api-openapi.yml
  format: yaml
  label: Leadspace Results API
  slug: leadspace-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadspace/refs/heads/main/openapi/leadspace-results-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Leadspace Authentication
name_suffix: Authentication
oauth_flows:
- password
- authorizationCode
overview: Leadspace secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password and authorizationCode flow(s).
provider_name: Leadspace
provider_slug: leadspace
scheme_count: 3
schemes:
- description: Perpetual token issued by Leadspace at program setup. Used directly as a bearer credential on every enrichment, discovery, and intent request.
  format: 'Authorization: Bearer API_KEY'
  in: header
  name: bearerAuth
  parameter: Authorization
  scheme: bearer
  sources:
  - openapi/leadspace-enrichment-openapi.yml
  - openapi/leadspace-discovery-openapi.yml
  - openapi/leadspace-intent-openapi.yml
  type: http
- audience: API_GATEWAY
  description: Username-password (resource owner password credentials) flow. POST the Program ID as `user`, the authentication secret as `pass`, and the audience `API_GATEWAY` to the authorize endpoint to receive a bearer token plus a refreshToken. Tokens expire every 24 hours; refresh with a PUT to the same endpoint.
  flow: password
  name: oauth2
  refreshUrl: https://apigw.leadspace.com/oauth/authorize
  scopes: []
  scopes_note: Leadspace does not document an OAuth scope surface; entitlement is bound to the Program ID rather than to per-request scopes.
  sources:
  - https://support.leadspace.com/hc/en-us/articles/360000827409-API-v4-OAuth-2-0-Diagram
  tokenUrl: https://apigw.leadspace.com/oauth/authorize
  token_ttl_seconds: 86400
  type: oauth2
- applies_to: https://skprod.leadspace.com/mcp/v1
  authorizationUrl: https://stg-sk.us.auth0.com/authorize
  bearer_methods_supported:
  - header
  challenge_observed: 'WWW-Authenticate: Bearer realm="leadspace-builders", resource_metadata="https://skprod.leadspace.com/mcp/v1/.well-known/oauth-protected-resource"'
  description: Per-USER OAuth for the Leadspace MCP server. The MCP client is registered dynamically (RFC 7591) — Leadspace's own setup instructions say to leave the OAuth client ID and secret fields blank — then the user signs in with their Leadspace account (the same account as Leadspace Sidekick; a free account can be created self-serve with a work email).
  discovery:
    authorization_server_metadata: https://skprod.leadspace.com/.well-known/oauth-authorization-server
    protected_resource_metadata: https://skprod.leadspace.com/.well-known/oauth-protected-resource
    spec:
    - RFC 9728
    - RFC 8414
    - RFC 7591
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://stg-sk.us.auth0.com/
  jwks_uri: https://stg-sk.us.auth0.com/.well-known/jwks.json
  name: mcp-oauth
  pkce: S256
  protocol: OAuth 2.1
  realm: leadspace-builders
  registrationUrl: https://stg-sk.us.auth0.com/oidc/register
  scopes:
  - openid
  - profile
  - email
  - offline_access
  scopes_note: Identity scopes only — there is no Leadspace-defined authorization scope. Entitlement (plan tier, credit balance, which reveals are allowed) is enforced server-side against the account, not by the token. Detail in scopes/leadspace-scopes.yml.
  sources:
  - https://www.leadspace.com/solutions/leadspace-mcp/claude
  - https://www.leadspace.com/solutions/leadspace-mcp/chatgpt
  - https://skprod.leadspace.com/.well-known/oauth-protected-resource
  tokenUrl: https://stg-sk.us.auth0.com/oauth/token
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  type: oauth2
slug: leadspace-authentication
source_filename: leadspace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://support.leadspace.com/hc/en-us/articles/23687993264284-Leadspace-Single-Direct-API-v4-Technical-Specifications\ndocs: https://support.leadspace.com/hc/en-us/articles/360000827409-API-v4-OAuth-2-0-Diagram\nupdate_note: >-\n  UPGRADE 2026-08-13. Leadspace now runs TWO unrelated authentication stacks.\n  The enterprise v4 gateway (apigw.leadspace.com) is unchanged: a Leadspace-issued\n  Program ID plus a perpetual bearer token, or an OAuth 2.0 resource-owner\n  password-credentials exchange against the gateway. The new Leadspace MCP server\n  (skprod.leadspace.com/mcp/v1) authenticates END USERS with OAuth 2.1\n  authorization-code + PKCE against an Auth0 tenant, with dynamic client\n  registration and RFC 9728 protected-resource metadata. A credential for one\n  does not work on the other.\nsummary:\n  types:\n    - http\n    - oauth2\n  api_key_in:\n    - header\n  oauth2_flows:\n    - password\n    - authorizationCode\n\
  \  transport: https-only\n  credential_delivery: >-\n    Leadspace issues a Program ID (username) and an authentication secret / API\n    key out of band, by email, at program setup. A customer may hold multiple\n    API keys, one per program.\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    in: header\n    parameter: Authorization\n    format: \"Authorization: Bearer API_KEY\"\n    description: >-\n      Perpetual token issued by Leadspace at program setup. Used directly as a\n      bearer credential on every enrichment, discovery, and intent request.\n    sources:\n      - openapi/leadspace-enrichment-openapi.yml\n      - openapi/leadspace-discovery-openapi.yml\n      - openapi/leadspace-intent-openapi.yml\n  - name: oauth2\n    type: oauth2\n    flow: password\n    description: >-\n      Username-password (resource owner password credentials) flow. POST the\n      Program ID as `user`, the authentication secret as `pass`, and the\n      audience `API_GATEWAY`\
  \ to the authorize endpoint to receive a bearer\n      token plus a refreshToken. Tokens expire every 24 hours; refresh with a\n      PUT to the same endpoint.\n    tokenUrl: https://apigw.leadspace.com/oauth/authorize\n    refreshUrl: https://apigw.leadspace.com/oauth/authorize\n    token_ttl_seconds: 86400\n    audience: API_GATEWAY\n    scopes: []\n    scopes_note: >-\n      Leadspace does not document an OAuth scope surface; entitlement is bound\n      to the Program ID rather than to per-request scopes.\n    sources:\n      - https://support.leadspace.com/hc/en-us/articles/360000827409-API-v4-OAuth-2-0-Diagram\n  - name: mcp-oauth\n    type: oauth2\n    flow: authorizationCode\n    applies_to: https://skprod.leadspace.com/mcp/v1\n    protocol: OAuth 2.1\n    pkce: S256\n    description: >-\n      Per-USER OAuth for the Leadspace MCP server. The MCP client is registered\n      dynamically (RFC 7591) — Leadspace's own setup instructions say to leave\n      the OAuth client ID and secret\
  \ fields blank — then the user signs in with\n      their Leadspace account (the same account as Leadspace Sidekick; a free\n      account can be created self-serve with a work email).\n    authorizationUrl: https://stg-sk.us.auth0.com/authorize\n    tokenUrl: https://stg-sk.us.auth0.com/oauth/token\n    registrationUrl: https://stg-sk.us.auth0.com/oidc/register\n    jwks_uri: https://stg-sk.us.auth0.com/.well-known/jwks.json\n    issuer: https://stg-sk.us.auth0.com/\n    grant_types:\n      - authorization_code\n      - refresh_token\n    token_endpoint_auth_methods:\n      - none\n      - client_secret_post\n    bearer_methods_supported:\n      - header\n    realm: leadspace-builders\n    scopes:\n      - openid\n      - profile\n      - email\n      - offline_access\n    scopes_note: >-\n      Identity scopes only — there is no Leadspace-defined authorization scope.\n      Entitlement (plan tier, credit balance, which reveals are allowed) is\n      enforced server-side against the account,\
  \ not by the token. Detail in\n      scopes/leadspace-scopes.yml.\n    discovery:\n      protected_resource_metadata: https://skprod.leadspace.com/.well-known/oauth-protected-resource\n      authorization_server_metadata: https://skprod.leadspace.com/.well-known/oauth-authorization-server\n      spec:\n        - RFC 9728\n        - RFC 8414\n        - RFC 7591\n    challenge_observed: 'WWW-Authenticate: Bearer realm=\"leadspace-builders\", resource_metadata=\"https://skprod.leadspace.com/mcp/v1/.well-known/oauth-protected-resource\"'\n    sources:\n      - https://www.leadspace.com/solutions/leadspace-mcp/claude\n      - https://www.leadspace.com/solutions/leadspace-mcp/chatgpt\n      - https://skprod.leadspace.com/.well-known/oauth-protected-resource\ntoken_rotation:\n  perpetual_token: true\n  recommended_rotation_months: 6\n  hard_expiry_years: 2\n  process: >-\n    Leadspace recommends rotating the perpetual token every six months from the\n    end of the integration period. An unrotated\
  \ token expires two years after\n    issue. Leadspace generates the replacement, notifies the customer ahead of\n    the end of the token lifecycle (10 working days' notice per the Discovery\n    API docs), and deprecates the old token once migration is confirmed.\nfailure_modes:\n  - status: 401\n    meaning: Wrong credentials, or credentials have expired\n  - status: 403\n    meaning: Program ID is invalid (Discovery API)\n  - status: 427\n    meaning: Insufficient credits, or the program ID is invalid\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leadspace/refs/heads/main/authentication/leadspace-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- MCP
- AI Agents
- B2B Data
- Customer Data Platform
- Data Enrichment
- Intent Data
- Sales Intelligence
- Account-Based Marketing
- Identity Resolution
- Firmographics
- Lead Scoring
- Company
---
