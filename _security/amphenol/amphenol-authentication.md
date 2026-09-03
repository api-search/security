---
api_key_in: []
auth_types: []
description: 'Amphenol publishes no developer authentication documentation, and there is no API key programme, signup or console anywhere on its sites. Two authentication postures were nevertheless observed directly on live Amphenol endpoints, and they sit at opposite ends: one surface is fully anonymous, the other is a standards-compliant OAuth 2.1 flow.'
kind: authentication
layout: security
method: probed
name: Amphenol Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amphenol declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Amphenol
provider_slug: amphenol
scheme_count: 2
schemes:
- description: No credential of any kind. A plain GET with a searchTerm query parameter returns HTTP 200 and a JSON body of distributor stock rows. No API key, no bearer token, no cookie, no nonce, no Origin restriction was observed.
  endpoint: https://amphenol-industrial.com/wp-json/parts-direct-search/v1/search
  evidence:
    content_type: application/json; charset=UTF-8
    status: 200
    url: https://amphenol-industrial.com/wp-json/parts-direct-search/v1/search?searchTerm=RADSOK
  id: none
  surface: Amphenol Industrial Parts Direct Search
  type: none
- bearer_methods_supported:
  - header
  description: OAuth 2.0 authorization-code flow with PKCE, advertised through RFC 8414 authorization server metadata and RFC 9728 protected resource metadata. The token endpoint accepts public clients (token_endpoint_auth_methods_supported is ["none"]) and the server supports client ID metadata documents, so a client can register itself by URL rather than out-of-band. Bearer token is presented in the Authorization header.
  endpoint: https://amphenol-automotive.com/wp-json/mcp/mcp-oauth-server
  evidence:
    body: '{"code":"mcp_unauthorized","message":"MCP authentication required."}'
    status: 401
    url: https://amphenol-automotive.com/wp-json/mcp/mcp-oauth-server
  flows:
    authorizationCode:
      authorizationUrl: https://amphenol-automotive.com/oauth/authorize
      pkce:
        methods:
        - S256
        required: true
      refreshSupported: true
      revocationUrl: https://amphenol-automotive.com/oauth/revoke
      scopes:
        mcp: Access to the Model Context Protocol resource
      tokenUrl: https://amphenol-automotive.com/oauth/token
  id: oauth2
  surface: Amphenol Automotive MCP server
  type: oauth2
slug: amphenol-authentication
source_filename: amphenol-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: >-\n  live probes of amphenol-automotive.com/.well-known/oauth-authorization-server,\n  amphenol-automotive.com/.well-known/oauth-protected-resource and\n  amphenol-industrial.com/wp-json/parts-direct-search/v1/search\nprovider: Amphenol\nproviderId: amphenol\ndescription: >-\n  Amphenol publishes no developer authentication documentation, and there is no API key\n  programme, signup or console anywhere on its sites. Two authentication postures were\n  nevertheless observed directly on live Amphenol endpoints, and they sit at opposite ends:\n  one surface is fully anonymous, the other is a standards-compliant OAuth 2.1 flow.\nschemes:\n  - id: none\n    type: none\n    surface: Amphenol Industrial Parts Direct Search\n    endpoint: https://amphenol-industrial.com/wp-json/parts-direct-search/v1/search\n    description: >-\n      No credential of any kind. A plain GET with a searchTerm query parameter returns HTTP 200\n      and\
  \ a JSON body of distributor stock rows. No API key, no bearer token, no cookie, no\n      nonce, no Origin restriction was observed.\n    evidence:\n      url: https://amphenol-industrial.com/wp-json/parts-direct-search/v1/search?searchTerm=RADSOK\n      status: 200\n      content_type: application/json; charset=UTF-8\n  - id: oauth2\n    type: oauth2\n    surface: Amphenol Automotive MCP server\n    endpoint: https://amphenol-automotive.com/wp-json/mcp/mcp-oauth-server\n    description: >-\n      OAuth 2.0 authorization-code flow with PKCE, advertised through RFC 8414 authorization\n      server metadata and RFC 9728 protected resource metadata. The token endpoint accepts\n      public clients (token_endpoint_auth_methods_supported is [\"none\"]) and the server supports\n      client ID metadata documents, so a client can register itself by URL rather than\n      out-of-band. Bearer token is presented in the Authorization header.\n    flows:\n      authorizationCode:\n        authorizationUrl:\
  \ https://amphenol-automotive.com/oauth/authorize\n        tokenUrl: https://amphenol-automotive.com/oauth/token\n        revocationUrl: https://amphenol-automotive.com/oauth/revoke\n        refreshSupported: true\n        pkce:\n          required: true\n          methods:\n            - S256\n        scopes:\n          mcp: Access to the Model Context Protocol resource\n    bearer_methods_supported:\n      - header\n    evidence:\n      url: https://amphenol-automotive.com/wp-json/mcp/mcp-oauth-server\n      status: 401\n      body: '{\"code\":\"mcp_unauthorized\",\"message\":\"MCP authentication required.\"}'\ndocs: null\ndocs_note: >-\n  No authentication documentation is published. Both schemes above were established by probing,\n  not by reading a page. www.amphenol.com returns HTTP 403 at the CDN edge to non-browser\n  clients, so a documentation page there could not be checked by this run.\nmaintainers:\n  - FN: API Evangelist\n    email: info@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amphenol/refs/heads/main/authentication/amphenol-authentication.yml
summary_line: 2 schemes
tags:
- Electronic Connectors
- Interconnect Systems
- Fiber Optics
- Sensors
- Aerospace
- Automotive
- Defense
- Manufacturing
- Fortune 500
---
