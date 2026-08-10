---
api_key_in: []
auth_types:
- none
- http
- oauth2
description: 'Cloud9 publishes no developer program and therefore no authentication documentation of its own. This profile was read from the live surface: the WordPress REST discovery index advertises its own authentication block, and the /.well-known/ OAuth metadata describes the MCP server''s authorization model. Three distinct postures coexist on the same host — anonymous read, application-password write, and OAuth 2.1 for MCP.'
kind: authentication
layout: security
method: probed
name: Cloud9 Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Cloud9 secures its APIs with none, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Cloud9
provider_slug: cloud9
scheme_count: 4
schemes:
- applies_to: https://cloud9.gg/wp-json/wp/v2/*
  description: Every wp/v2 content collection returns 200 to an unauthenticated GET — posts, pages, media, users, categories, tags, search, and the Cloud9 custom post types players, teams, achievement and case-study. No key, no header, no referrer check. Verified against 14 collections.
  name: AnonymousRead
  sources:
  - https://cloud9.gg/wp-json/
  type: none
- applies_to: write operations on https://cloud9.gg/wp-json/wp/v2/*
  authorization_endpoint: https://cloud9.gg/wp-admin/authorize-application.php
  description: The discovery index declares authentication.application-passwords with an authorization endpoint at https://cloud9.gg/wp-admin/authorize-application.php. Application passwords are sent as HTTP Basic credentials (username + generated application password) and inherit the WordPress user's roles and capabilities. Only site users can obtain one — this is not a public developer credential.
  name: WordPressApplicationPasswords
  scheme: basic
  sources:
  - https://cloud9.gg/wp-json/
  type: http
- applies_to: https://cloud9.gg/wp-json/mcp/mcp-oauth-server
  description: OAuth 2.1 authorization code with PKCE (S256) for the remote MCP server. Public clients (token_endpoint_auth_method none), refresh tokens supported, single `mcp` scope, bearer token in the Authorization header. On an unauthenticated call the server returns a conformant RFC 9728 challenge naming the protected-resource metadata document.
  detail: scopes/cloud9-scopes.yml
  flows:
  - authorizationUrl: https://cloud9.gg/oauth/authorize
    flow: authorizationCode
    revocationUrl: https://cloud9.gg/oauth/revoke
    scopes: 1
    tokenUrl: https://cloud9.gg/oauth/token
  issuer: https://cloud9.gg
  name: Cloud9MCPOAuth
  sources:
  - https://cloud9.gg/.well-known/oauth-authorization-server
  type: oauth2
- applies_to: https://store.cloud9.gg/products.json
  description: The Shopify storefront JSON endpoints answer anonymously. Cloud9 exposes no Storefront API access token publicly and no Admin API surface.
  name: ShopifyStorefrontAnonymous
  sources:
  - https://store.cloud9.gg/products.json
  type: none
slug: cloud9-authentication
source_filename: cloud9-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: https://cloud9.gg/wp-json/ + https://cloud9.gg/.well-known/oauth-authorization-server\ndocs: https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/\ndescription: >-\n  Cloud9 publishes no developer program and therefore no authentication documentation of its own.\n  This profile was read from the live surface: the WordPress REST discovery index advertises its\n  own authentication block, and the /.well-known/ OAuth metadata describes the MCP server's\n  authorization model. Three distinct postures coexist on the same host — anonymous read,\n  application-password write, and OAuth 2.1 for MCP.\nsummary:\n  types: [none, http, oauth2]\n  anonymous_read: true\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: AnonymousRead\n  type: none\n  applies_to: https://cloud9.gg/wp-json/wp/v2/*\n  description: >-\n    Every wp/v2 content collection returns 200 to an unauthenticated GET — posts,\
  \ pages, media,\n    users, categories, tags, search, and the Cloud9 custom post types players, teams,\n    achievement and case-study. No key, no header, no referrer check. Verified against 14\n    collections.\n  sources: [https://cloud9.gg/wp-json/]\n- name: WordPressApplicationPasswords\n  type: http\n  scheme: basic\n  applies_to: write operations on https://cloud9.gg/wp-json/wp/v2/*\n  description: >-\n    The discovery index declares authentication.application-passwords with an authorization\n    endpoint at https://cloud9.gg/wp-admin/authorize-application.php. Application passwords are\n    sent as HTTP Basic credentials (username + generated application password) and inherit the\n    WordPress user's roles and capabilities. Only site users can obtain one — this is not a\n    public developer credential.\n  authorization_endpoint: https://cloud9.gg/wp-admin/authorize-application.php\n  sources: [https://cloud9.gg/wp-json/]\n- name: Cloud9MCPOAuth\n  type: oauth2\n  applies_to:\
  \ https://cloud9.gg/wp-json/mcp/mcp-oauth-server\n  description: >-\n    OAuth 2.1 authorization code with PKCE (S256) for the remote MCP server. Public clients\n    (token_endpoint_auth_method none), refresh tokens supported, single `mcp` scope, bearer\n    token in the Authorization header. On an unauthenticated call the server returns a\n    conformant RFC 9728 challenge naming the protected-resource metadata document.\n  issuer: https://cloud9.gg\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://cloud9.gg/oauth/authorize\n    tokenUrl: https://cloud9.gg/oauth/token\n    revocationUrl: https://cloud9.gg/oauth/revoke\n    scopes: 1\n  detail: scopes/cloud9-scopes.yml\n  sources: [https://cloud9.gg/.well-known/oauth-authorization-server]\n- name: ShopifyStorefrontAnonymous\n  type: none\n  applies_to: https://store.cloud9.gg/products.json\n  description: >-\n    The Shopify storefront JSON endpoints answer anonymously. Cloud9 exposes no Storefront API\n    access token\
  \ publicly and no Admin API surface.\n  sources: [https://store.cloud9.gg/products.json]\nnot_found:\n  api_keys: No API key programme, developer portal, or key-issuance flow exists on any Cloud9 host.\n  openid_connect: https://cloud9.gg/.well-known/openid-configuration returns 404.\n  mutual_tls: Not advertised.\nx-evidence:\n  fetched: '2026-08-09'\n  probes:\n  - url: https://cloud9.gg/wp-json/\n    status: 200\n    finding: 'authentication: {application-passwords: {endpoints: {authorization: .../authorize-application.php}}}'\n  - url: https://cloud9.gg/wp-json/wp/v2/players?per_page=1\n    status: 200\n    finding: anonymous read succeeds\n  - url: https://cloud9.gg/.well-known/oauth-authorization-server\n    status: 200\n  - url: https://cloud9.gg/wp-json/mcp/mcp-oauth-server\n    method: POST tools/list\n    status: 401\n  - url: https://cloud9.gg/.well-known/openid-configuration\n    status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloud9/refs/heads/main/authentication/cloud9-authentication.yml
summary_line: none/http/oauth2 · 4 schemes
tags:
- Company
- Esports
- Gaming
- Entertainment
- Media
- Sports
- Content
- WordPress
- Community
- Merchandise
---
