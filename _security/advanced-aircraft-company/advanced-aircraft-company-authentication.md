---
anonymous_access: true
api_key_in: []
auth_types: []
description: 'Advanced Aircraft Company publishes no authentication documentation of its own. This profile is read entirely from machine-readable documents its host actually serves: the `authentication` block of the WordPress REST API discovery root and the two OAuth discovery documents published by the WordPress MCP Adapter. Two distinct schemes are in play on the same origin.'
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Advanced Aircraft Company Authentication
name_suffix: Authentication
oauth_flows: []
overview: Advanced Aircraft Company declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Advanced Aircraft Company
provider_slug: advanced-aircraft-company
scheme_count: 3
schemes:
- applies_to: WordPress core content namespace (wp/v2, oembed/1.0)
  description: The public content surface requires no credentials. GET /wp-json/wp/v2/posts, /pages, /media, /categories and /types all return 200 with no Authorization header.
  id: anonymous-read
  type: none
  verified:
    http_status: 200
    url: https://advancedaircraftcompany.com/wp-json/wp/v2/posts?per_page=1
- applies_to: All write operations and the ~511 plugin/admin routes (aioseo, jetpack, google-site-kit, redirection, wp-rocket, newfold/bluehost, wpforms, wp-abilities, mcp, blu).
  authorization_url: https://advancedaircraftcompany.com/wp-admin/authorize-application.php
  description: WordPress Application Passwords, the only scheme the discovery root advertises. Credentials are issued interactively by a logged-in site administrator; there is no self-service developer signup.
  id: application-passwords
  scheme: basic
  source: wp-json authentication.application-passwords.endpoints.authorization
  type: http
  verified:
    http_status: 401
    response_code: rest_forbidden
    url: https://advancedaircraftcompany.com/wp-json/wp-abilities/v1/abilities
- applies_to: The MCP server at /wp-json/mcp/mcp-oauth-server
  authorization_endpoint: https://advancedaircraftcompany.com/oauth/authorize
  bearer_methods_supported:
  - header
  code_challenge_methods:
  - S256
  description: OAuth 2.1-shaped authorization code flow with mandatory PKCE, published as RFC 8414 authorization server metadata and RFC 9728 protected resource metadata. Public clients only (token_endpoint_auth_methods_supported is ["none"]). Dynamic client registration is NOT offered; instead client_id_metadata_document_supported is true, so a client identifies itself by a URL pointing at its own metadata document.
  grant_types:
  - authorization_code
  - refresh_token
  id: mcp-oauth
  issuer: https://advancedaircraftcompany.com
  response_types:
  - code
  revocation_endpoint: https://advancedaircraftcompany.com/oauth/revoke
  scopes:
  - mcp
  token_endpoint: https://advancedaircraftcompany.com/oauth/token
  type: oauth2
  verified:
    http_status: 401
    response_code: mcp_unauthorized
    url: https://advancedaircraftcompany.com/wp-json/mcp/mcp-oauth-server
slug: advanced-aircraft-company-authentication
source_filename: advanced-aircraft-company-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: >-\n  https://advancedaircraftcompany.com/wp-json (authentication block),\n  https://advancedaircraftcompany.com/.well-known/oauth-authorization-server,\n  https://advancedaircraftcompany.com/.well-known/oauth-protected-resource\nname: Advanced Aircraft Company Authentication Profile\ndescription: >-\n  Advanced Aircraft Company publishes no authentication documentation of its own. This profile is read\n  entirely from machine-readable documents its host actually serves: the `authentication` block of the\n  WordPress REST API discovery root and the two OAuth discovery documents published by the WordPress\n  MCP Adapter. Two distinct schemes are in play on the same origin.\nschemes:\n- id: anonymous-read\n  type: none\n  applies_to: WordPress core content namespace (wp/v2, oembed/1.0)\n  description: >-\n    The public content surface requires no credentials. GET /wp-json/wp/v2/posts, /pages, /media,\n    /categories and /types\
  \ all return 200 with no Authorization header.\n  verified:\n    url: https://advancedaircraftcompany.com/wp-json/wp/v2/posts?per_page=1\n    http_status: 200\n- id: application-passwords\n  type: http\n  scheme: basic\n  applies_to: >-\n    All write operations and the ~511 plugin/admin routes (aioseo, jetpack, google-site-kit,\n    redirection, wp-rocket, newfold/bluehost, wpforms, wp-abilities, mcp, blu).\n  description: >-\n    WordPress Application Passwords, the only scheme the discovery root advertises. Credentials are\n    issued interactively by a logged-in site administrator; there is no self-service developer signup.\n  authorization_url: https://advancedaircraftcompany.com/wp-admin/authorize-application.php\n  source: wp-json authentication.application-passwords.endpoints.authorization\n  verified:\n    url: https://advancedaircraftcompany.com/wp-json/wp-abilities/v1/abilities\n    http_status: 401\n    response_code: rest_forbidden\n- id: mcp-oauth\n  type: oauth2\n  applies_to:\
  \ The MCP server at /wp-json/mcp/mcp-oauth-server\n  description: >-\n    OAuth 2.1-shaped authorization code flow with mandatory PKCE, published as RFC 8414 authorization\n    server metadata and RFC 9728 protected resource metadata. Public clients only\n    (token_endpoint_auth_methods_supported is [\"none\"]). Dynamic client registration is NOT offered;\n    instead client_id_metadata_document_supported is true, so a client identifies itself by a URL\n    pointing at its own metadata document.\n  issuer: https://advancedaircraftcompany.com\n  authorization_endpoint: https://advancedaircraftcompany.com/oauth/authorize\n  token_endpoint: https://advancedaircraftcompany.com/oauth/token\n  revocation_endpoint: https://advancedaircraftcompany.com/oauth/revoke\n  response_types: [code]\n  grant_types: [authorization_code, refresh_token]\n  code_challenge_methods: [S256]\n  bearer_methods_supported: [header]\n  scopes: [mcp]\n  verified:\n    url: https://advancedaircraftcompany.com/wp-json/mcp/mcp-oauth-server\n\
  \    http_status: 401\n    response_code: mcp_unauthorized\nnotes:\n- No OpenID Connect. /.well-known/openid-configuration returns 404 with the site's HTML theme shell.\n- No API key scheme, no mutual TLS, no signed requests.\n- >-\n  There is no developer signup. The only account surface on the site is a Simple WP Membership\n  investor portal (/membership-login/), which is unrelated to API access.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advanced-aircraft-company/refs/heads/main/authentication/advanced-aircraft-company-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Aerospace
- Defense
- Drones
- Unmanned Aircraft Systems
- UAV
- VTOL
- Manufacturing
- Public Safety
- Content
---
