---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Chord Commerce Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chord declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Chord
provider_slug: chord-commerce
scheme_count: 4
schemes:
- api: Chord MCP
  authorization_endpoint: https://hub-backend.chord.co/oauth/authorize
  bearer_methods:
  - header
  challenge: '401 with WWW-Authenticate: Bearer resource_metadata="https://mcp.chord.co/.well-known/oauth-protected-resource/mcp"'
  docs: https://docs.chord.co/chord-mcp
  dynamic_client_registration: true
  evidence: probed 2026-08-13; both discovery documents returned HTTP 200
  flow: authorization_code
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: mcp-oauth
  issuer: https://api.stytch.chord.co
  jwks_uri: https://api.stytch.chord.co/.well-known/jwks.json
  note: 'Standards-clean MCP auth: RFC 9728 protected-resource metadata, RFC 8414 authorization-server metadata, RFC 7591 dynamic client registration, PKCE S256. Chord''s docs tell users to leave the optional OAuth Client ID/Secret blank — registration is dynamic. Authorization is per-USER, scoped to the Chord organizations that account belongs to; there is no service account.'
  pkce_methods:
  - S256
  registration_endpoint: https://api.stytch.chord.co/v1/oauth2/register
  resource: https://mcp.chord.co/mcp
  scopes:
  - openid
  - profile
  - email
  - offline_access
  token_endpoint: https://api.stytch.chord.co/v1/oauth2/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
  userinfo_endpoint: https://api.stytch.chord.co/v1/oauth2/userinfo
- additional_required_header:
    description: The unique user identifier used as the `pk` in the customer's audience sync — Chord recommends the CDP Blended User ID. The API returns 401 Unauthorized without a valid bearer token.
    name: Chord-User-Id
  api: Chord Audiences API
  docs: https://docs.chord.co/audiences-api
  evidence: probed 2026-08-13 — GET https://analytics.api.chord.co/audiences returned HTTP 401 {"message":"Unauthorized"}; the host root returns HTTP 403 {"message":"Missing Authentication Token"} (AWS API Gateway default).
  header: 'Authorization: Bearer <api key>'
  id: audiences-bearer
  key_issuance: Keys are issued by Chord staff on request (help@chord.co or the account executive); there is no self-service key console documented.
  note: Server-side only. Chord's own docs state the Audiences API "should always be called server-side", so the bearer token must never reach a browser.
  scheme: bearer
  type: http
- alternatives:
  - in: query
    name: writekey
    note: all lowercase
  - in: body
    name: writeKey
    note: capital K
  api: Chord CDP Ingest API
  docs: https://docs.chord.co/server-events-overview
  id: cdp-write-key
  in: header
  name: X-Write-Key
  note: A per-source write key, the Segment/Jitsu convention. Chord explicitly recommends the header form over the query-string and body forms, both of which are offered only for source systems that cannot set headers — the query-string variant leaks the credential into access logs.
  preferred: X-Write-Key header
  type: apiKey
- api: Chord Platform (hub.chord.co)
  docs: https://docs.chord.co/chord-platform-and-okta-sso-integration
  id: platform-saml-sso
  idp_documented: Okta
  note: SAML 2.0 SSO for human access to the Chord console, set up by Chord support from the customer's IdP metadata. This is console auth, not API auth — no SCIM provisioning endpoint is documented.
  type: saml2
slug: chord-commerce-authentication
source_filename: chord-commerce-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://docs.chord.co/server-events-overview, https://docs.chord.co/audiences-api,\n  https://docs.chord.co/chord-mcp, https://mcp.chord.co/.well-known/oauth-protected-resource,\n  https://api.stytch.chord.co/.well-known/openid-configuration\nnote: >-\n  Chord publishes no OpenAPI, so this profile is transcribed from the docs and\n  from live probes of the OAuth/OIDC discovery documents rather than derived from\n  securitySchemes. Three distinct API surfaces, three different auth models — an\n  agent cannot assume one credential works across them.\nschemes:\n  - id: mcp-oauth\n    api: Chord MCP\n    type: oauth2\n    flow: authorization_code\n    pkce_methods:\n      - S256\n    dynamic_client_registration: true\n    issuer: https://api.stytch.chord.co\n    authorization_endpoint: https://hub-backend.chord.co/oauth/authorize\n    token_endpoint: https://api.stytch.chord.co/v1/oauth2/token\n    registration_endpoint:\
  \ https://api.stytch.chord.co/v1/oauth2/register\n    userinfo_endpoint: https://api.stytch.chord.co/v1/oauth2/userinfo\n    jwks_uri: https://api.stytch.chord.co/.well-known/jwks.json\n    grant_types:\n      - authorization_code\n      - refresh_token\n      - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n    token_endpoint_auth_methods:\n      - client_secret_basic\n      - client_secret_post\n      - none\n    bearer_methods:\n      - header\n    scopes:\n      - openid\n      - profile\n      - email\n      - offline_access\n    resource: https://mcp.chord.co/mcp\n    challenge: >-\n      401 with WWW-Authenticate: Bearer\n      resource_metadata=\"https://mcp.chord.co/.well-known/oauth-protected-resource/mcp\"\n    docs: https://docs.chord.co/chord-mcp\n    evidence: probed 2026-08-13; both discovery documents returned HTTP 200\n    note: >-\n      Standards-clean MCP auth: RFC 9728 protected-resource metadata, RFC 8414\n      authorization-server metadata, RFC 7591 dynamic client\
  \ registration, PKCE\n      S256. Chord's docs tell users to leave the optional OAuth Client ID/Secret\n      blank — registration is dynamic. Authorization is per-USER, scoped to the\n      Chord organizations that account belongs to; there is no service account.\n  - id: audiences-bearer\n    api: Chord Audiences API\n    type: http\n    scheme: bearer\n    header: 'Authorization: Bearer <api key>'\n    additional_required_header:\n      name: Chord-User-Id\n      description: >-\n        The unique user identifier used as the `pk` in the customer's audience\n        sync — Chord recommends the CDP Blended User ID. The API returns 401\n        Unauthorized without a valid bearer token.\n    key_issuance: >-\n      Keys are issued by Chord staff on request (help@chord.co or the account\n      executive); there is no self-service key console documented.\n    docs: https://docs.chord.co/audiences-api\n    evidence: >-\n      probed 2026-08-13 — GET https://analytics.api.chord.co/audiences\
  \ returned\n      HTTP 401 {\"message\":\"Unauthorized\"}; the host root returns HTTP 403\n      {\"message\":\"Missing Authentication Token\"} (AWS API Gateway default).\n    note: >-\n      Server-side only. Chord's own docs state the Audiences API \"should always be\n      called server-side\", so the bearer token must never reach a browser.\n  - id: cdp-write-key\n    api: Chord CDP Ingest API\n    type: apiKey\n    in: header\n    name: X-Write-Key\n    alternatives:\n      - in: query\n        name: writekey\n        note: all lowercase\n      - in: body\n        name: writeKey\n        note: capital K\n    preferred: X-Write-Key header\n    docs: https://docs.chord.co/server-events-overview\n    note: >-\n      A per-source write key, the Segment/Jitsu convention. Chord explicitly\n      recommends the header form over the query-string and body forms, both of\n      which are offered only for source systems that cannot set headers — the\n      query-string variant leaks the credential\
  \ into access logs.\n  - id: platform-saml-sso\n    api: Chord Platform (hub.chord.co)\n    type: saml2\n    idp_documented: Okta\n    docs: https://docs.chord.co/chord-platform-and-okta-sso-integration\n    note: >-\n      SAML 2.0 SSO for human access to the Chord console, set up by Chord support\n      from the customer's IdP metadata. This is console auth, not API auth — no\n      SCIM provisioning endpoint is documented.\ngaps:\n  - No published key-rotation policy for the Audiences API bearer token or the CDP write key.\n  - No self-service credential management surface is documented for any of the three APIs.\n  - No mTLS, no signed-request scheme, no HMAC webhook signature documented.\n  - >-\n    Audiences API and CDP ingest keys are both long-lived shared secrets with no\n    documented scope model; only the MCP surface has scoped, revocable, per-user\n    credentials.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chord-commerce/refs/heads/main/authentication/chord-commerce-authentication.yml
summary_line: 4 schemes
tags:
- Commerce
- Composable Commerce
- Headless Commerce
- Order Management
- OMS
- Customer Data Platform
- CDP
- Event Tracking
- Commerce Analytics
- Customer Lifetime Value
- AI Agents
- Commerce Copilot
- Solidus
- Spree
- Ruby On Rails
- Shopify
- DTC
- Direct To Consumer
---
