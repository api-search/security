---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Stagwell Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stagwell declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Stagwell
provider_slug: stagwell
scheme_count: 2
schemes:
- applies_to: IMAI Discovery API, IMAI Raw API
  base_url: https://imai.co/api
  confidence: medium
  confidence_note: The header name and key style are stated on the public API page and by the provider's own documentation index, but the full reference at https://imai.co/documentation is a client-rendered Angular application that serves no machine-readable contract to an anonymous client, so parameter-level detail could not be verified.
  evidence: The published API page documents an Authorization header carrying an API key; https://imai.co/api answers HTTP 403 with the plain body "Unauthorized" to an anonymous request, and the IMAI web application bundle (https://imai.co/main.a29b2d4cf73bd5fe.js) carries https://imai.co/api as the production API root (with https://dev.influencermarketing.ai/api as the development root).
  id: imai-api-key
  in: header
  name: Authorization
  obtained_via: Contract-based sale only. The provider states "we currently do not offer monthly or pay-as-you-go plans. All plans are contract-based", and testing credits are issued by an account manager after a scheduled call — there is no self-serve API key issuance.
  source: https://influencermarketing.ai/api/
  type: apiKey
- applies_to: IMAI MCP server (Novamira)
  bearer_methods_supported:
  - header
  confidence: high
  confidence_note: Read verbatim from anonymous RFC 8414 / OIDC discovery documents served by the provider; saved to well-known/.
  dynamic_client_registration: https://influencermarketing.ai/wp-json/novamira/v1/oauth/register
  flows:
  - authorizationUrl: https://influencermarketing.ai/wp-admin/admin.php?page=novamira-oauth-authorize
    flow: authorizationCode
    pkce: S256
    scopes:
      mcp: Access the site's Model Context Protocol server
    tokenUrl: https://influencermarketing.ai/wp-json/novamira/v1/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  id: novamira-oauth2
  introspection_endpoint: https://influencermarketing.ai/wp-json/novamira/v1/oauth/introspect
  issuer: https://influencermarketing.ai
  protected_resource: https://influencermarketing.ai/wp-json/mcp/novamira-oauth
  response_types_supported:
  - code
  revocation_endpoint: https://influencermarketing.ai/wp-json/novamira/v1/oauth/revoke
  source: https://influencermarketing.ai/.well-known/oauth-authorization-server
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
slug: stagwell-authentication
source_filename: stagwell-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://influencermarketing.ai/api/\ndocs: https://imai.co/documentation\nnote: >-\n  Stagwell (the holding company) publishes no developer authentication surface of\n  its own. Two distinct auth models exist on Stagwell-owned properties, both on\n  IMAI / InfluencerMarketing.ai (a Stagwell company since the July 2024 LEADERS\n  acquisition, inside the PRophet suite of the Stagwell Marketing Cloud): an API\n  key for the IMAI Discovery/Raw product APIs, and a full OAuth 2.0 authorization\n  server for the site's MCP endpoint. No OpenAPI is published, so none of this is\n  derived from a spec — it is read from the provider's own pages and from live\n  anonymous discovery documents.\nschemes:\n  - id: imai-api-key\n    applies_to: IMAI Discovery API, IMAI Raw API\n    type: apiKey\n    in: header\n    name: Authorization\n    base_url: https://imai.co/api\n    obtained_via: >-\n      Contract-based sale only. The provider states\
  \ \"we currently do not offer\n      monthly or pay-as-you-go plans. All plans are contract-based\", and testing\n      credits are issued by an account manager after a scheduled call — there is\n      no self-serve API key issuance.\n    source: https://influencermarketing.ai/api/\n    evidence: >-\n      The published API page documents an Authorization header carrying an API\n      key; https://imai.co/api answers HTTP 403 with the plain body \"Unauthorized\"\n      to an anonymous request, and the IMAI web application bundle\n      (https://imai.co/main.a29b2d4cf73bd5fe.js) carries https://imai.co/api as\n      the production API root (with https://dev.influencermarketing.ai/api as the\n      development root).\n    confidence: medium\n    confidence_note: >-\n      The header name and key style are stated on the public API page and by the\n      provider's own documentation index, but the full reference at\n      https://imai.co/documentation is a client-rendered Angular application\
  \ that\n      serves no machine-readable contract to an anonymous client, so parameter-level\n      detail could not be verified.\n  - id: novamira-oauth2\n    applies_to: IMAI MCP server (Novamira)\n    type: oauth2\n    protected_resource: https://influencermarketing.ai/wp-json/mcp/novamira-oauth\n    issuer: https://influencermarketing.ai\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://influencermarketing.ai/wp-admin/admin.php?page=novamira-oauth-authorize\n        tokenUrl: https://influencermarketing.ai/wp-json/novamira/v1/oauth/token\n        pkce: S256\n        scopes:\n          mcp: Access the site's Model Context Protocol server\n    grant_types_supported: [authorization_code, refresh_token]\n    response_types_supported: [code]\n    token_endpoint_auth_methods_supported: [none]\n    bearer_methods_supported: [header]\n    dynamic_client_registration: https://influencermarketing.ai/wp-json/novamira/v1/oauth/register\n    revocation_endpoint: https://influencermarketing.ai/wp-json/novamira/v1/oauth/revoke\n\
  \    introspection_endpoint: https://influencermarketing.ai/wp-json/novamira/v1/oauth/introspect\n    source: https://influencermarketing.ai/.well-known/oauth-authorization-server\n    confidence: high\n    confidence_note: >-\n      Read verbatim from anonymous RFC 8414 / OIDC discovery documents served by\n      the provider; saved to well-known/.\nmtls: false\nopenid_connect:\n  discovery: https://influencermarketing.ai/.well-known/openid-configuration\n  note: >-\n    An OIDC-shaped discovery document is served, but it advertises only the\n    OAuth 2.0 code flow for the \"mcp\" scope — no id_token, userinfo or jwks\n    endpoints are present, so this is OAuth 2.0 discovery published at the OIDC\n    path rather than a conformant OpenID Provider.\nx-evidence:\n  fetched: '2026-08-12'\n  probes:\n    - url: https://imai.co/api\n      status: 403\n      response: Unauthorized\n    - url: https://influencermarketing.ai/.well-known/oauth-authorization-server\n      status: 200\n    - url:\
  \ https://influencermarketing.ai/.well-known/openid-configuration\n      status: 200\n    - url: https://influencermarketing.ai/api/\n      status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stagwell/refs/heads/main/authentication/stagwell-authentication.yml
summary_line: 2 schemes
tags:
- Marketing
- Advertising
- Media
- MarTech
- Influencer Marketing
- Market Research
- Creator Economy
- Public Relations
- Consumer Insights
- Holding Company
---
