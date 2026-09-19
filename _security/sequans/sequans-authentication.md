---
anonymous_access: false
api_key_in: []
auth_types:
- oauth2
description: 'Sequans publishes no developer program and no authentication documentation. This profile was read from the live sequans.com surface: the RFC 8414 / RFC 9728 metadata served by the WordPress MCP Adapter describes the MCP server''s authorization model, and the WordPress REST index lists no authentication methods of its own (its `authentication` block is empty). Product documentation, SDKs and firmware sit behind the my.sequans.com support-zone account, which is a customer web login, not an API credential.'
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Sequans Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Sequans secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Sequans
provider_slug: sequans
scheme_count: 2
schemes:
- applies_to: https://sequans.com/wp-json/mcp/mcp-oauth-server
  description: OAuth 2.1 authorization code with PKCE (S256) for the remote MCP server. Public clients (token_endpoint_auth_method none), refresh tokens supported, client ID metadata documents supported, single `mcp` scope, bearer token in the Authorization header. An unauthenticated call returns 401 with an RFC 9728 challenge naming the protected-resource metadata document.
  detail: scopes/sequans-scopes.yml
  flows:
  - authorizationUrl: https://sequans.com/oauth/authorize
    flow: authorizationCode
    revocationUrl: https://sequans.com/oauth/revoke
    scopes: 1
    tokenUrl: https://sequans.com/oauth/token
  issuer: https://sequans.com
  name: SequansMCPOAuth
  sources:
  - https://sequans.com/.well-known/oauth-authorization-server
  - https://sequans.com/.well-known/oauth-protected-resource
  type: oauth2
- applies_to: https://sequans.com/wp-json/mcp/mcp-adapter-default-server
  description: The default MCP adapter server answers anonymous calls with 401 rest_forbidden and no OAuth challenge, meaning it is gated by WordPress user capabilities (a logged-in site user) rather than by the OAuth server above.
  name: WordPressSession
  sources:
  - https://sequans.com/wp-json/mcp/mcp-adapter-default-server
  type: other
slug: sequans-authentication
source_filename: sequans-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: probed\nsource: https://sequans.com/.well-known/oauth-authorization-server + https://sequans.com/wp-json/\ndocs: null\ndescription: >-\n  Sequans publishes no developer program and no authentication documentation. This profile was\n  read from the live sequans.com surface: the RFC 8414 / RFC 9728 metadata served by the WordPress\n  MCP Adapter describes the MCP server's authorization model, and the WordPress REST index lists no\n  authentication methods of its own (its `authentication` block is empty). Product documentation,\n  SDKs and firmware sit behind the my.sequans.com support-zone account, which is a customer web\n  login, not an API credential.\nsummary:\n  types: [oauth2]\n  anonymous_read: false\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: SequansMCPOAuth\n  type: oauth2\n  applies_to: https://sequans.com/wp-json/mcp/mcp-oauth-server\n  description: >-\n    OAuth 2.1 authorization code with PKCE (S256)\
  \ for the remote MCP server. Public clients\n    (token_endpoint_auth_method none), refresh tokens supported, client ID metadata documents\n    supported, single `mcp` scope, bearer token in the Authorization header. An unauthenticated\n    call returns 401 with an RFC 9728 challenge naming the protected-resource metadata document.\n  issuer: https://sequans.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sequans.com/oauth/authorize\n    tokenUrl: https://sequans.com/oauth/token\n    revocationUrl: https://sequans.com/oauth/revoke\n    scopes: 1\n  detail: scopes/sequans-scopes.yml\n  sources: [https://sequans.com/.well-known/oauth-authorization-server, https://sequans.com/.well-known/oauth-protected-resource]\n- name: WordPressSession\n  type: other\n  applies_to: https://sequans.com/wp-json/mcp/mcp-adapter-default-server\n  description: >-\n    The default MCP adapter server answers anonymous calls with 401 rest_forbidden and no OAuth\n    challenge, meaning\
  \ it is gated by WordPress user capabilities (a logged-in site user) rather\n    than by the OAuth server above.\n  sources: [https://sequans.com/wp-json/mcp/mcp-adapter-default-server]\nnot_found:\n  api_keys: No API key programme, developer portal or key-issuance flow exists on any Sequans host.\n  openid_connect: https://sequans.com/.well-known/openid-configuration returns 404.\n  mutual_tls: Not advertised.\n  dynamic_client_registration: No RFC 7591 registration_endpoint is advertised.\nx-evidence:\n  fetched: '2026-09-16'\n  probes:\n  - url: https://sequans.com/.well-known/oauth-authorization-server\n    status: 200\n  - url: https://sequans.com/.well-known/oauth-protected-resource\n    status: 200\n  - url: https://sequans.com/.well-known/openid-configuration\n    status: 404\n  - url: https://sequans.com/wp-json/\n    status: 200\n  - url: https://sequans.com/wp-json/mcp/mcp-oauth-server\n    status: 401\n  - url: https://sequans.com/wp-json/mcp/mcp-adapter-default-server\n  \
  \  status: 401\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sequans/refs/heads/main/authentication/sequans-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Semiconductors
- Cellular IoT
- 5G
- LTE-M
- NB-IoT
- IoT Modules
- Hardware
- Telecommunications
- France
---
