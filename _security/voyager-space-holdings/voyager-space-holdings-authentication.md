---
anonymous_access: false
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Voyager Space Holdings Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Voyager Technologies secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Voyager Technologies
provider_slug: voyager-space-holdings
scheme_count: 2
schemes:
- challenge:
    http_status: 401
    observed_on: https://voyagertechnologies.com/wp-json/mcp/mcp-oauth-server
    www_authenticate: Bearer realm="https://voyagertechnologies.com", resource_metadata="https://voyagertechnologies.com/.well-known/oauth-protected-resource"
  description: OAuth 2.1 authorization-code + PKCE (S256), as advertised by the provider's RFC 8414 metadata. grant_types_supported [authorization_code, refresh_token]; response_types_supported [code]; token_endpoint_auth_methods_supported ["none"] (public client); client_id_metadata_document_supported true (clients identify with a hosted metadata URL rather than a pre-registered client_id); authorization_response_iss_parameter_supported true; a revocation endpoint at /oauth/revoke. The RFC 9728 document names the protected resource https://voyagertechnologies.com/wp-json/mcp/mcp-oauth-server with bearer_methods_supported ["header"].
  flows:
  - authorizationUrl: https://voyagertechnologies.com/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://voyagertechnologies.com/oauth/token
    scopes:
      mcp: Access the site's Model Context Protocol server (the only scope advertised in scopes_supported).
    tokenUrl: https://voyagertechnologies.com/oauth/token
  name: mcpOAuth2
  sources:
  - well-known/voyager-space-holdings-oauth-authorization-server.json
  - well-known/voyager-space-holdings-oauth-protected-resource.json
  type: oauth2
- description: WordPress cookie-authentication nonce, advertised by the live server in its Access-Control-Allow-Headers response header (Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type). Only meaningful for a logged-in WordPress session; not a public credential path.
  in: header
  name: wpNonce
  parameter: X-WP-Nonce
  sources:
  - https://voyagertechnologies.com/wp-json/mcp/mcp-oauth-server
  type: apiKey
slug: voyager-space-holdings-authentication
source_filename: voyager-space-holdings-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: searched\nsource: https://voyagertechnologies.com/.well-known/oauth-authorization-server\ndocs: null\nnote: >-\n  No OpenAPI exists to derive from, so this profile is read directly from the two OAuth discovery\n  documents the provider's host serves (RFC 8414 and RFC 9728, both HTTP 200 on 2026-09-18) and\n  from the WWW-Authenticate challenge observed on the MCP endpoint. It describes the WordPress MCP\n  adapter's authorization server, the only authenticated machine surface on the domain; the\n  company publishes no product API, no API keys and no developer authentication documentation.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  pkce: required\n  public_client: true\nschemes:\n- name: mcpOAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://voyagertechnologies.com/oauth/authorize\n    tokenUrl: https://voyagertechnologies.com/oauth/token\n    refreshUrl: https://voyagertechnologies.com/oauth/token\n\
  \    scopes:\n      mcp: Access the site's Model Context Protocol server (the only scope advertised in scopes_supported).\n  description: >-\n    OAuth 2.1 authorization-code + PKCE (S256), as advertised by the provider's RFC 8414 metadata.\n    grant_types_supported [authorization_code, refresh_token]; response_types_supported [code];\n    token_endpoint_auth_methods_supported [\"none\"] (public client);\n    client_id_metadata_document_supported true (clients identify with a hosted metadata URL rather\n    than a pre-registered client_id); authorization_response_iss_parameter_supported true; a\n    revocation endpoint at /oauth/revoke. The RFC 9728 document names the protected resource\n    https://voyagertechnologies.com/wp-json/mcp/mcp-oauth-server with bearer_methods_supported\n    [\"header\"].\n  sources:\n  - well-known/voyager-space-holdings-oauth-authorization-server.json\n  - well-known/voyager-space-holdings-oauth-protected-resource.json\n  challenge:\n    observed_on: https://voyagertechnologies.com/wp-json/mcp/mcp-oauth-server\n\
  \    http_status: 401\n    www_authenticate: Bearer realm=\"https://voyagertechnologies.com\", resource_metadata=\"https://voyagertechnologies.com/.well-known/oauth-protected-resource\"\n- name: wpNonce\n  type: apiKey\n  in: header\n  parameter: X-WP-Nonce\n  description: >-\n    WordPress cookie-authentication nonce, advertised by the live server in its\n    Access-Control-Allow-Headers response header (Authorization, X-WP-Nonce, Content-Disposition,\n    Content-MD5, Content-Type). Only meaningful for a logged-in WordPress session; not a public\n    credential path.\n  sources:\n  - https://voyagertechnologies.com/wp-json/mcp/mcp-oauth-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voyager-space-holdings/refs/heads/main/authentication/voyager-space-holdings-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Space
- Defense
- Aerospace
- Propulsion
- Satellite
- Lunar
- Space Stations
- Public Company
---
