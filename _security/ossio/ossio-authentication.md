---
api_key_in: []
auth_types: []
description: OSSIO publishes no product API and no developer authentication documentation. The one authenticated surface it serves is the site MCP server, whose auth profile is fully described by the RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata documents saved in well-known/. Everything below is read from those documents.
kind: authentication
layout: security
method: probed
name: Ossio Authentication
name_suffix: Authentication
oauth_flows: []
overview: OSSIO declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: OSSIO
provider_slug: ossio
scheme_count: 2
schemes:
- applies_to:
  - https://ossio.io/wp-json/mcp/mcp-oauth-server
  authorization_endpoint: https://ossio.io/oauth/authorize
  client_registration:
    dynamic: true
    mechanism: client_id_metadata_document
    note: client_id_metadata_document_supported is true and token_endpoint_auth_methods_supported is ["none"], i.e. public clients identified by a hosted client-metadata document rather than a pre-registered secret. No RFC 7591 registration_endpoint is advertised.
  flow: authorization_code
  grant_types_supported:
  - authorization_code
  - refresh_token
  id: oauth2_mcp
  issuer: https://ossio.io
  pkce:
    code_challenge_methods_supported:
    - S256
    required: true
  response_types_supported:
  - code
  revocation_endpoint: https://ossio.io/oauth/revoke
  scopes:
  - mcp
  token_endpoint: https://ossio.io/oauth/token
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
- applies_to:
  - https://ossio.io/wp-json/mcp/mcp-adapter-default-server
  - https://ossio.io/wp-json/wp-abilities/v1/abilities
  flow: null
  id: wordpress_rest
  note: /wp-json/mcp/mcp-adapter-default-server, /wp-json/wp-abilities/v1/* and the private WordPress REST routes reject anonymous calls with rest_forbidden (HTTP 401), i.e. they expect a WordPress cookie+nonce or an application password. This is WordPress core behaviour, not a documented OSSIO auth product.
  type: apiKey
slug: ossio-authentication
source_filename: ossio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://ossio.io/.well-known/oauth-authorization-server\nname: OSSIO Authentication Profile\ndescription: >-\n  OSSIO publishes no product API and no developer authentication documentation. The one\n  authenticated surface it serves is the site MCP server, whose auth profile is fully\n  described by the RFC 8414 authorization-server metadata and RFC 9728 protected-resource\n  metadata documents saved in well-known/. Everything below is read from those documents.\nschemes:\n- id: oauth2_mcp\n  type: oauth2\n  flow: authorization_code\n  issuer: https://ossio.io\n  authorization_endpoint: https://ossio.io/oauth/authorize\n  token_endpoint: https://ossio.io/oauth/token\n  revocation_endpoint: https://ossio.io/oauth/revoke\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  pkce:\n    required: true\n    code_challenge_methods_supported:\n    - S256\n  token_endpoint_auth_methods_supported:\n\
  \  - none\n  client_registration:\n    dynamic: true\n    mechanism: client_id_metadata_document\n    note: >-\n      client_id_metadata_document_supported is true and token_endpoint_auth_methods_supported\n      is [\"none\"], i.e. public clients identified by a hosted client-metadata document\n      rather than a pre-registered secret. No RFC 7591 registration_endpoint is advertised.\n  scopes:\n  - mcp\n  applies_to:\n  - https://ossio.io/wp-json/mcp/mcp-oauth-server\n- id: wordpress_rest\n  type: apiKey\n  flow: null\n  note: >-\n    /wp-json/mcp/mcp-adapter-default-server, /wp-json/wp-abilities/v1/* and the private\n    WordPress REST routes reject anonymous calls with rest_forbidden (HTTP 401), i.e. they\n    expect a WordPress cookie+nonce or an application password. This is WordPress core\n    behaviour, not a documented OSSIO auth product.\n  applies_to:\n  - https://ossio.io/wp-json/mcp/mcp-adapter-default-server\n  - https://ossio.io/wp-json/wp-abilities/v1/abilities\nanonymous_surface:\n\
  \  note: >-\n    Parts of the WordPress REST API are readable anonymously (e.g. /wp-json/wp/v2/types,\n    HTTP 200). These are CMS content routes, not an OSSIO API product.\ndocs: null\ndocs_note: OSSIO publishes no authentication documentation page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ossio/refs/heads/main/authentication/ossio-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Medical Devices
- Health
- Orthopedics
- Life Sciences
- Manufacturing
- MCP
- Agents
---
