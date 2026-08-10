---
api_key_in: []
auth_types: []
description: Cardiosense publishes no developer API and no authentication documentation. The authentication profile below is not derived from an OpenAPI securitySchemes block — there is no OpenAPI — it is read directly from the two OAuth discovery documents the host serves anonymously, plus the authentication block of the public WordPress REST route index.
kind: authentication
layout: security
method: probed
name: Cardiosense Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cardiosense declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Cardiosense
provider_slug: cardiosense
scheme_count: 2
schemes:
- applies_to: https://cardiosense.com/wp-json/mcp/mcp-oauth-server
  authorization_endpoint: https://cardiosense.com/oauth/authorize
  bearer_methods_supported:
  - header
  client_identification: client_id_metadata_document_supported = true. No RFC 7591 dynamic client registration endpoint is advertised, so a client is identified by a URL pointing at its own client-ID metadata document.
  code_challenge_methods_supported:
  - S256
  evidence:
    http_status: 200
    url: https://cardiosense.com/.well-known/oauth-authorization-server
  flow: authorization_code
  grant_types_supported:
  - authorization_code
  - refresh_token
  id: mcp_oauth2
  issuer: https://cardiosense.com
  observations:
  - PKCE is mandatory in practice — S256 is the only challenge method offered and no client secret method is supported.
  - Public-client only (`none`); there is no confidential-client path.
  - A refresh_token grant is offered, but no token lifetime or rotation policy is published.
  - No id_token / OpenID Connect layer — /.well-known/openid-configuration returns 404.
  response_types_supported:
  - code
  revocation_endpoint: https://cardiosense.com/oauth/revoke
  scopes:
  - mcp
  token_endpoint: https://cardiosense.com/oauth/token
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
- applies_to: https://cardiosense.com/wp-json/
  description: The WordPress REST API index advertises Application Passwords as its authentication mechanism, authorized at https://cardiosense.com/wp-admin/authorize-application.php. This is a WordPress platform default rather than a Cardiosense product decision, and it gates the CMS content routes and the default MCP server.
  evidence:
    http_status: 200
    url: https://cardiosense.com/wp-json/
  id: wp_application_passwords
  scheme: basic
  type: http
slug: cardiosense-authentication
source_filename: cardiosense-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: https://cardiosense.com/.well-known/oauth-authorization-server\ndescription: >-\n  Cardiosense publishes no developer API and no authentication documentation.\n  The authentication profile below is not derived from an OpenAPI\n  securitySchemes block — there is no OpenAPI — it is read directly from the\n  two OAuth discovery documents the host serves anonymously, plus the\n  authentication block of the public WordPress REST route index.\ndocs: null\ndocs_note: >-\n  There is no published auth guide. Everything here came from machine-readable\n  discovery documents, not from prose a developer could read.\n\nschemes:\n  - id: mcp_oauth2\n    type: oauth2\n    flow: authorization_code\n    applies_to: https://cardiosense.com/wp-json/mcp/mcp-oauth-server\n    issuer: https://cardiosense.com\n    authorization_endpoint: https://cardiosense.com/oauth/authorize\n    token_endpoint: https://cardiosense.com/oauth/token\n    revocation_endpoint:\
  \ https://cardiosense.com/oauth/revoke\n    response_types_supported: [code]\n    grant_types_supported: [authorization_code, refresh_token]\n    code_challenge_methods_supported: [S256]\n    token_endpoint_auth_methods_supported: [none]\n    bearer_methods_supported: [header]\n    scopes: [mcp]\n    client_identification: >-\n      client_id_metadata_document_supported = true. No RFC 7591 dynamic client\n      registration endpoint is advertised, so a client is identified by a URL\n      pointing at its own client-ID metadata document.\n    observations:\n      - PKCE is mandatory in practice — S256 is the only challenge method offered and no client secret method is supported.\n      - Public-client only (`none`); there is no confidential-client path.\n      - A refresh_token grant is offered, but no token lifetime or rotation policy is published.\n      - No id_token / OpenID Connect layer — /.well-known/openid-configuration returns 404.\n    evidence:\n      url: https://cardiosense.com/.well-known/oauth-authorization-server\n\
  \      http_status: 200\n\n  - id: wp_application_passwords\n    type: http\n    scheme: basic\n    applies_to: https://cardiosense.com/wp-json/\n    description: >-\n      The WordPress REST API index advertises Application Passwords as its\n      authentication mechanism, authorized at\n      https://cardiosense.com/wp-admin/authorize-application.php. This is a\n      WordPress platform default rather than a Cardiosense product decision,\n      and it gates the CMS content routes and the default MCP server.\n    evidence:\n      url: https://cardiosense.com/wp-json/\n      http_status: 200\n\nanonymous_access:\n  - surface: https://cardiosense.com/llms.txt\n    authenticated: false\n    status: 200\n  - surface: https://cardiosense.com/wp-json/ (route index)\n    authenticated: false\n    status: 200\n  - surface: https://cardiosense.com/wp-json/mcp/mcp-oauth-server\n    authenticated: true\n    status: 401\n  - surface: https://cardiosense.com/wp-json/wp-abilities/v1/abilities\n   \
  \ authenticated: true\n    status: 401\n\ngaps:\n  - No human-readable authentication documentation exists for the MCP surface.\n  - No dynamic client registration endpoint, so onboarding an agent client requires an out-of-band conversation with Cardiosense.\n  - Token lifetimes, refresh rotation, and scope semantics for `mcp` are undocumented.\n\nx-evidence:\n  fetched: '2026-08-09'\n  probes:\n    - url: https://cardiosense.com/.well-known/oauth-authorization-server\n      status: 200\n    - url: https://cardiosense.com/.well-known/oauth-protected-resource\n      status: 200\n    - url: https://cardiosense.com/.well-known/openid-configuration\n      status: 404\n    - url: https://cardiosense.com/wp-json/\n      status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cardiosense/refs/heads/main/authentication/cardiosense-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Health
- Digital Health
- Medical Devices
- Cardiology
- Heart Failure
- Remote Patient Monitoring
- Wearables
- Artificial Intelligence
- Machine Learning
- Model Context Protocol
---
