---
api_key_in: []
auth_types: []
description: Reed Semiconductor publishes no OpenAPI and no authentication documentation — it runs no developer program. This profile is built entirely from live probes of the REST and MCP surfaces its WordPress deployment serves, and from the OAuth metadata documents at /.well-known/. Three distinct authentication regimes coexist on one host.
kind: authentication
layout: security
method: probed
name: Reed Semiconductor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reed Semiconductor declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Reed Semiconductor
provider_slug: reed-semiconductor
scheme_count: 4
schemes:
- applies_to:
  - https://www.reedsemi.com/wp-json/wc/store/v1/products
  - https://www.reedsemi.com/wp-json/wc/store/v1/products/categories
  - https://www.reedsemi.com/wp-json/wc/store/v1/products/brands
  - https://www.reedsemi.com/wp-json/wp/v2/posts
  - https://www.reedsemi.com/wp-json/wp/v2/pages
  - https://www.reedsemi.com/wp-json/wp/v2/media
  description: 'Public read. The WooCommerce Store API product catalog and the WordPress content API answer anonymously with HTTP 200 and no credential of any kind. Verified against /wc/store/v1/products (99 items, X-WP-Total: 99) and /wp/v2/posts (10 items).'
  id: none
  type: none
  verified: probed
- applies_to:
  - https://www.reedsemi.com/wp-json/mcp/novamira-oauth
  - https://www.reedsemi.com/wp-json/wp-abilities/v1/abilities
  bearer_methods:
  - header
  challenge_observed: 'WWW-Authenticate: Bearer resource_metadata="https://www.reedsemi.com/.well-known/oauth-protected-resource", scope="mcp"'
  description: 'OAuth 2.1 bearer tokens, advertised via RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata. Authorization-code with mandatory PKCE S256, refresh tokens, and the RFC 8628 device-code grant. Public clients (token_endpoint_auth_methods: none) with open RFC 7591 dynamic client registration. Single scope: mcp. Bearer token is presented in the Authorization header.'
  id: oauth2
  issuer: https://www.reedsemi.com
  scopes:
  - mcp
  type: oauth2
  verified: probed
- applies_to:
  - https://www.reedsemi.com/wp-json/wp/v2/
  authorization_endpoint: https://www.reedsemi.com/wp-admin/authorize-application.php
  description: WordPress Application Passwords, advertised in the /wp-json/ root discovery document under authentication.application-passwords. Used for authenticated writes to the content API. Authorization page is /wp-admin/authorize-application.php.
  id: wordpress-application-passwords
  scheme: basic
  type: http
  verified: probed
- applies_to:
  - https://www.reedsemi.com/wp-json/mcp/novamira
  - https://www.reedsemi.com/wp-json/mcp/mcp-adapter-default-server
  - https://www.reedsemi.com/wp-json/novamira/v1/
  description: Cookie + nonce authentication for same-origin, logged-in WordPress sessions. The two non-OAuth MCP servers and the Novamira admin routes reject anonymous calls with rest_forbidden under this regime. Not usable by an external agent.
  id: wordpress-cookie-nonce
  in: header
  name: X-WP-Nonce
  type: apiKey
  verified: probed
slug: reed-semiconductor-authentication
source_filename: reed-semiconductor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://www.reedsemi.com/wp-json/\nname: Reed Semiconductor Authentication\ndescription: >-\n  Reed Semiconductor publishes no OpenAPI and no authentication documentation — it runs\n  no developer program. This profile is built entirely from live probes of the REST and\n  MCP surfaces its WordPress deployment serves, and from the OAuth metadata documents at\n  /.well-known/. Three distinct authentication regimes coexist on one host.\nderived_from: probes\nschemes:\n- id: none\n  type: none\n  applies_to:\n  - https://www.reedsemi.com/wp-json/wc/store/v1/products\n  - https://www.reedsemi.com/wp-json/wc/store/v1/products/categories\n  - https://www.reedsemi.com/wp-json/wc/store/v1/products/brands\n  - https://www.reedsemi.com/wp-json/wp/v2/posts\n  - https://www.reedsemi.com/wp-json/wp/v2/pages\n  - https://www.reedsemi.com/wp-json/wp/v2/media\n  description: >-\n    Public read. The WooCommerce Store API product catalog and the\
  \ WordPress content\n    API answer anonymously with HTTP 200 and no credential of any kind. Verified against\n    /wc/store/v1/products (99 items, X-WP-Total: 99) and /wp/v2/posts (10 items).\n  verified: probed\n- id: oauth2\n  type: oauth2\n  applies_to:\n  - https://www.reedsemi.com/wp-json/mcp/novamira-oauth\n  - https://www.reedsemi.com/wp-json/wp-abilities/v1/abilities\n  description: >-\n    OAuth 2.1 bearer tokens, advertised via RFC 8414 authorization-server metadata and\n    RFC 9728 protected-resource metadata. Authorization-code with mandatory PKCE S256,\n    refresh tokens, and the RFC 8628 device-code grant. Public clients\n    (token_endpoint_auth_methods: none) with open RFC 7591 dynamic client registration.\n    Single scope: mcp. Bearer token is presented in the Authorization header.\n  issuer: https://www.reedsemi.com\n  bearer_methods:\n  - header\n  scopes:\n  - mcp\n  challenge_observed: >-\n    WWW-Authenticate: Bearer\n    resource_metadata=\"https://www.reedsemi.com/.well-known/oauth-protected-resource\"\
  ,\n    scope=\"mcp\"\n  verified: probed\n- id: wordpress-application-passwords\n  type: http\n  scheme: basic\n  applies_to:\n  - https://www.reedsemi.com/wp-json/wp/v2/\n  description: >-\n    WordPress Application Passwords, advertised in the /wp-json/ root discovery document\n    under authentication.application-passwords. Used for authenticated writes to the\n    content API. Authorization page is /wp-admin/authorize-application.php.\n  authorization_endpoint: https://www.reedsemi.com/wp-admin/authorize-application.php\n  verified: probed\n- id: wordpress-cookie-nonce\n  type: apiKey\n  in: header\n  name: X-WP-Nonce\n  applies_to:\n  - https://www.reedsemi.com/wp-json/mcp/novamira\n  - https://www.reedsemi.com/wp-json/mcp/mcp-adapter-default-server\n  - https://www.reedsemi.com/wp-json/novamira/v1/\n  description: >-\n    Cookie + nonce authentication for same-origin, logged-in WordPress sessions. The two\n    non-OAuth MCP servers and the Novamira admin routes reject anonymous calls\
  \ with\n    rest_forbidden under this regime. Not usable by an external agent.\n  verified: probed\ncors:\n  access_control_allow_headers:\n  - Authorization\n  - X-WP-Nonce\n  - Content-Disposition\n  - Content-MD5\n  - Content-Type\n  - Cart-Token\n  - Nonce\n  access_control_expose_headers:\n  - X-WP-Total\n  - X-WP-TotalPages\n  - Link\n  - Cart-Token\nfindings:\n  public_read: true\n  oauth_present: true\n  api_keys: false\n  mtls: false\n  openid_connect_claim: >-\n    An /.well-known/openid-configuration document is served, but it is byte-identical to\n    the OAuth authorization-server metadata: no jwks_uri, no userinfo_endpoint, no\n    id_token signing algorithms, no subject types. It advertises OAuth, not OIDC.\n    Treat the OIDC discovery path as an alias, not as OpenID Connect support.\nx-evidence:\n  fetched: '2026-08-26'\n  probes:\n  - url: https://www.reedsemi.com/wp-json/\n    status: 200\n  - url: https://www.reedsemi.com/wp-json/wc/store/v1/products?per_page=3\n  \
  \  status: 200\n  - url: https://www.reedsemi.com/wp-json/wp/v2/posts?per_page=10\n    status: 200\n  - url: https://www.reedsemi.com/wp-json/mcp/novamira-oauth\n    status: 401\n  - url: https://www.reedsemi.com/wp-json/mcp/novamira\n    status: 401\n  - url: https://www.reedsemi.com/wp-json/wp-abilities/v1/abilities\n    status: 401\n  - url: https://www.reedsemi.com/.well-known/openid-configuration\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reed-semiconductor/refs/heads/main/authentication/reed-semiconductor-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Semiconductors
- Power Management
- Electronic Components
- Data-Center
- Artificial Intelligence
- Automotive
- Hardware
- Manufacturing
- Product Catalog
---
