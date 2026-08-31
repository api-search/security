---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Techsee Authentication
name_suffix: Authentication
oauth_flows: []
overview: TechSee declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: TechSee
provider_slug: techsee
scheme_count: 2
schemes:
- applies_to: mcp
  authorization_url: https://techsee.com/oauth/authorize
  client_authentication: none
  client_authentication_note: token_endpoint_auth_methods_supported is ["none"] — public clients only, no client secret. client_id_metadata_document_supported is true, so a client is identified by a URL that resolves to its client-ID metadata document rather than by a pre-registered client_id/secret pair. No dynamic client registration endpoint (RFC 7591) is advertised.
  evidence:
    file: ../well-known/techsee-oauth-authorization-server.json
    status: 200
    url: https://techsee.com/.well-known/oauth-authorization-server
  flow: authorizationCode
  id: oauth2_mcp
  issuer: https://techsee.com
  pkce: required
  pkce_methods:
  - S256
  protects:
  - https://techsee.com/wp-json/mcp/mcp-oauth-server
  refresh: true
  revocation_url: https://techsee.com/oauth/revoke
  scopes:
  - mcp
  token_presentation: Authorization Bearer header (bearer_methods_supported ["header"])
  token_url: https://techsee.com/oauth/token
  type: oauth2
- applies_to: https://techsee.com/wp-json/
  documented: false
  evidence:
    status: 401
    url: https://techsee.com/wp-json/wp-abilities/v1/abilities
  id: wordpress_rest
  note: The non-OAuth MCP adapter server and the wp-abilities routes are gated by ordinary WordPress REST authentication; an unauthenticated GET returns {"code":"rest_forbidden","message":"Sorry, you are not allowed to do that."} with HTTP 401. Recorded as observed behaviour, not as a documented scheme.
  scheme: cookie-or-application-password
  type: http
slug: techsee-authentication
source_filename: techsee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: >-\n  https://techsee.com/.well-known/oauth-authorization-server (200, RFC 8414) and\n  https://techsee.com/.well-known/oauth-protected-resource (200, RFC 9728),\n  fetched 2026-08-29\nname: TechSee\nslug: techsee\nsummary: >-\n  TechSee publishes no public authentication documentation for its product API — the\n  developer portal is not reachable (see x-coverage). The one authentication model\n  that IS machine-readable and was verified by probe is the OAuth 2.0 authorization\n  server that fronts TechSee's MCP endpoint on techsee.com. Everything below is read\n  from those two live metadata documents, not from prose.\n\nschemes:\n- id: oauth2_mcp\n  type: oauth2\n  flow: authorizationCode\n  pkce: required\n  pkce_methods: [S256]\n  authorization_url: https://techsee.com/oauth/authorize\n  token_url: https://techsee.com/oauth/token\n  revocation_url: https://techsee.com/oauth/revoke\n  refresh: true\n  issuer: https://techsee.com\n\
  \  scopes:\n  - mcp\n  client_authentication: none\n  client_authentication_note: >-\n    token_endpoint_auth_methods_supported is [\"none\"] — public clients only, no\n    client secret. client_id_metadata_document_supported is true, so a client is\n    identified by a URL that resolves to its client-ID metadata document rather\n    than by a pre-registered client_id/secret pair. No dynamic client registration\n    endpoint (RFC 7591) is advertised.\n  token_presentation: Authorization Bearer header (bearer_methods_supported [\"header\"])\n  protects:\n  - https://techsee.com/wp-json/mcp/mcp-oauth-server\n  applies_to: mcp\n  evidence:\n    url: https://techsee.com/.well-known/oauth-authorization-server\n    status: 200\n    file: ../well-known/techsee-oauth-authorization-server.json\n\n- id: wordpress_rest\n  type: http\n  scheme: cookie-or-application-password\n  documented: false\n  applies_to: https://techsee.com/wp-json/\n  note: >-\n    The non-OAuth MCP adapter server and the wp-abilities\
  \ routes are gated by\n    ordinary WordPress REST authentication; an unauthenticated GET returns\n    {\"code\":\"rest_forbidden\",\"message\":\"Sorry, you are not allowed to do that.\"}\n    with HTTP 401. Recorded as observed behaviour, not as a documented scheme.\n  evidence:\n    url: https://techsee.com/wp-json/wp-abilities/v1/abilities\n    status: 401\n\nproduct_api:\n  documented: false\n  note: >-\n    TechSee markets an \"open integration platform\" of APIs and prebuilt CRM/CCaaS\n    connectors, but no public reference states how those APIs authenticate. The\n    former developer portal at https://techsee.readme.io/ answers 401, and the\n    Stoplight workspace at https://techsee.stoplight.io/ publishes zero public\n    projects. No API key, bearer, HMAC or OAuth scheme for the product API could be\n    observed, and none is asserted here.\n  evidence:\n  - url: https://techsee.readme.io/\n    status: 401\n  - url: https://techsee.stoplight.io/\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/techsee/refs/heads/main/authentication/techsee-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Visual Assistance
- Customer Experience
- Customer Service
- Contact Center
- Computer Vision
- Augmented Reality
- Artificial Intelligence
- Field Service
- Remote Support
- Video
- Telecommunications
---
