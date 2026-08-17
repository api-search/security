---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Newfold Authentication
name_suffix: Authentication
oauth_flows: []
overview: Newfold declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Newfold
provider_slug: newfold
scheme_count: 0
schemes: []
slug: newfold-authentication
source_filename: newfold-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://github.com/newfold-labs/wp-module-mcp/blob/main/docs/api.md\ndocs: https://www.npmjs.com/package/@newfold/wp-mcp-connector\nnote: 'Derived from first-party source and docs rather than from an OpenAPI — Newfold\n  publishes no public OpenAPI, so there are no securitySchemes to read. Everything\n  below is stated by Newfold in its own GPL source or package README.'\napis:\n- api: newfold:blu-mcp\n  surface: https://{site}/wp-json/blu/mcp\n  schemes:\n  - id: wordpress-capability\n    type: session\n    detail: 'Server side, the transport permission callback allows the request outright\n      when the caller is a logged-in WordPress user holding the manage_options capability.\n      This is the admin-in-browser path.'\n    source: includes/Validation/McpValidation.php\n  - id: hiive-jwt\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    algorithm: RS256\n    detail: 'Otherwise a Bearer JWT is required in\
  \ the Authorization header. Signatures\n      are verified with firebase/php-jwt against public keys fetched from the Hiive\n      CDN, so the issuer is Newfold''s own platform rather than the site.'\n    key_source: Hiive CDN public keys\n  - id: application-password\n    type: http\n    scheme: basic\n    detail: 'WordPress Application Passwords (Authorization: Basic) work when the request\n      authenticates as an administrator before the MCP permission callback runs. Newfold\n      documents this as the local-testing path and its CI evals provision one automatically\n      via wp-env + WP-CLI.'\n  - id: oauth21\n    type: oauth2\n    flow: authorization_code\n    detail: 'Client side, @newfold/wp-mcp-connector implements OAuth 2.1 against the\n      site. PKCE (S256) is always on for the authorization-code flow. Protected-resource\n      metadata (RFC 9728) is discovered first, falling back to authorization-server\n      metadata (RFC 8414) and then an unauthenticated probe of the\
  \ WWW-Authenticate\n      header. Dynamic client registration (RFC 7591) runs when no client id is supplied\n      and the server advertises a registration endpoint. Resource indicators (RFC 8707)\n      are sent unless disabled.'\n    default_scopes: [read, write]\n    legacy_flow: implicit (OAUTH_FLOW_TYPE=implicit, for older sites)\n    token_storage: '~/.newfold/wp-mcp-connector/v<version>/, file mode 0600, isolated\n      per site by MD5 of the site URL; a lockfile coordinates concurrent connector\n      instances so only one opens a browser.'\n  - id: woocommerce-keys\n    type: apiKey\n    detail: WooCommerce report tools (wc_reports_*) swap to WOO_CUSTOMER_KEY / WOO_CUSTOMER_SECRET\n      instead of the primary basic-auth credentials when invoked.\n  - id: custom-headers\n    type: apiKey\n    in: header\n    detail: When CUSTOM_HEADERS is the only auth source the connector forwards those\n      headers verbatim and sends no Authorization header, which is the escape hatch\n   \
  \   for API-key setups.\n- api: newfold:hiive\n  surface: https://hiive.cloud/api\n  schemes:\n  - id: hiive-site-token\n    type: http\n    scheme: bearer\n    detail: 'The wp-module-data connection exchanges a site token during the nfd-hiive-verify\n      handshake and sends it on subsequent requests to sites/v1/events and sites/v2/events.\n      Tokens are issued to the site by Newfold; there is no public self-service credential\n      issuance and no documented developer onboarding for this API.'\n    source: includes/HiiveConnection.php\n- api: newfold:huapi\n  surface: not published\n  schemes: []\n  note: 'The generated client (@newfold/huapi-js) carries no auth configuration of\n    its own — callers supply an axios instance. Newfold publishes no public auth documentation\n    for HUAPI.'\ngaps:\n- No public OAuth scope reference. The connector defaults to \"read,write\" and the actual\n  scope vocabulary is whatever each WordPress site's OAuth plugin advertises, so there\n  is\
  \ nothing provider-published to record in scopes/.\n- No /.well-known/oauth-authorization-server or /.well-known/oauth-protected-resource\n  is served by any Newfold-controlled host; discovery happens against the customer's\n  own site.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newfold/refs/heads/main/authentication/newfold-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Web Hosting
- Domains
- Web Presence
- Website Builder
- Digital Marketing
- Small Business
- WordPress
- Open Source
- Model Context Protocol
- eCommerce
---
