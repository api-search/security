---
api_key_in:
- header
api_specs:
- filename: redefine-meat-wc-store-v1-api-openapi.yml
  format: yaml
  label: Redefine Meat Wc/store/v1 API
  slug: redefine-meat-wc-store-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redefine-meat/refs/heads/main/openapi/redefine-meat-wc-store-v1-api-openapi.yml
- filename: redefine-meat-wp-v2-api-openapi.yml
  format: yaml
  label: Redefine Meat Wp/v2 API
  slug: redefine-meat-wp-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redefine-meat/refs/heads/main/openapi/redefine-meat-wp-v2-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Redefine Meat Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: Redefine Meat secures its APIs with apiKey, http, and oauth2 across 7 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: Redefine Meat
provider_slug: redefine-meat
scheme_count: 7
schemes:
- description: No credential required. Verified on /wc/store/v1/products (200), /wc/store/v1/products/categories (200), /wc/store/v1/cart (200) and /wp/v2/posts (200).
  name: anonymous
  sources:
  - https://www.redefinemeat.com/wp-json/wc/store/v1/products
  type: none
- description: Store API write operations require a valid Nonce header. Observed without it - HTTP 401 {"code":"woocommerce_rest_missing_nonce","message":"Missing the Nonce header. This endpoint requires a valid nonce."}
  in: header
  name: cartNonce
  parameter: Nonce
  sources:
  - openapi/redefine-meat-store-openapi.json
  type: apiKey
- description: Store API cart session token, exposed to browsers via the Cart-Token response header (access-control-expose-headers includes Cart-Token).
  in: header
  name: cartToken
  parameter: Cart-Token
  sources:
  - openapi/redefine-meat-store-openapi.json
  type: apiKey
- description: Cookie-authenticated WordPress REST requests require X-WP-Nonce. Declared in the host's access-control-allow-headers.
  in: header
  name: wpNonce
  parameter: X-WP-Nonce
  sources:
  - openapi/redefine-meat-content-openapi.json
  type: apiKey
- authorization_endpoint: https://www.redefinemeat.com/wp-admin/authorize-application.php
  description: WordPress Application Passwords (HTTP Basic). Declared by the site's own discovery index - authentication.application-passwords.endpoints.authorization = https://www.redefinemeat.com/wp-admin/authorize-application.php
  name: applicationPassword
  scheme: basic
  sources:
  - https://www.redefinemeat.com/wp-json/
  type: http
- description: OAuth 2.1 authorization-code flow with mandatory PKCE (S256) and public clients (token_endpoint_auth_methods_supported = none), protecting the Model Context Protocol endpoints. Client identity uses a client_id metadata document rather than dynamic registration.
  flows:
  - authorizationUrl: https://www.redefinemeat.com/oauth/authorize
    flow: authorizationCode
    revocationUrl: https://www.redefinemeat.com/oauth/revoke
    scopes:
    - mcp
    tokenUrl: https://www.redefinemeat.com/oauth/token
  - flow: refreshToken
    tokenUrl: https://www.redefinemeat.com/oauth/token
  name: mcpOAuth
  sources:
  - https://www.redefinemeat.com/.well-known/oauth-authorization-server
  type: oauth2
- description: The wc/v3, wc/v2 and wc/v1 namespaces are registered on this host (234 routes). WooCommerce normally authenticates these with consumer key/secret pairs, but nothing on this host documents or confirms that; an anonymous GET /wc/v3/products returned HTTP 401 {"code":"woocommerce_rest_cannot_view","message":"Sorry, you cannot list resources."}. Recorded as inferred, not asserted.
  in: query
  name: wooCommerceKeys
  parameter: consumer_key / consumer_secret
  sources:
  - https://www.redefinemeat.com/wp-json/
  status: inferred-not-verified
  type: apiKey
slug: redefine-meat-authentication
source_filename: redefine-meat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: >-\n  openapi/redefine-meat-store-openapi.json, openapi/redefine-meat-content-openapi.json,\n  https://www.redefinemeat.com/wp-json/,\n  https://www.redefinemeat.com/.well-known/oauth-authorization-server\ndocs: null\nnote: >-\n  Redefine Meat publishes no authentication documentation - it runs no developer program. Every\n  mechanism below was observed directly against the live host: the WordPress REST discovery\n  index declares Application Passwords, the CORS headers declare the accepted auth headers, and\n  the observed 401 envelopes name the exact missing credential.\nsummary:\n  types: [apiKey, http, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, refreshToken]\n  anonymous_read: true\n  anonymous_read_note: >-\n    The WooCommerce Store API read surface (products, categories, attributes, brands, tags,\n    reviews, cart) and the wp/v2 collection reads return HTTP 200 with no credential at all.\nschemes:\n\
  - name: anonymous\n  type: none\n  description: >-\n    No credential required. Verified on /wc/store/v1/products (200), /wc/store/v1/products/categories\n    (200), /wc/store/v1/cart (200) and /wp/v2/posts (200).\n  sources: [https://www.redefinemeat.com/wp-json/wc/store/v1/products]\n- name: cartNonce\n  type: apiKey\n  in: header\n  parameter: Nonce\n  description: >-\n    Store API write operations require a valid Nonce header. Observed without it -\n    HTTP 401 {\"code\":\"woocommerce_rest_missing_nonce\",\"message\":\"Missing the Nonce header.\n    This endpoint requires a valid nonce.\"}\n  sources: [openapi/redefine-meat-store-openapi.json]\n- name: cartToken\n  type: apiKey\n  in: header\n  parameter: Cart-Token\n  description: >-\n    Store API cart session token, exposed to browsers via the Cart-Token response header\n    (access-control-expose-headers includes Cart-Token).\n  sources: [openapi/redefine-meat-store-openapi.json]\n- name: wpNonce\n  type: apiKey\n  in: header\n\
  \  parameter: X-WP-Nonce\n  description: >-\n    Cookie-authenticated WordPress REST requests require X-WP-Nonce. Declared in the host's\n    access-control-allow-headers.\n  sources: [openapi/redefine-meat-content-openapi.json]\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: >-\n    WordPress Application Passwords (HTTP Basic). Declared by the site's own discovery index -\n    authentication.application-passwords.endpoints.authorization =\n    https://www.redefinemeat.com/wp-admin/authorize-application.php\n  authorization_endpoint: https://www.redefinemeat.com/wp-admin/authorize-application.php\n  sources: [https://www.redefinemeat.com/wp-json/]\n- name: mcpOAuth\n  type: oauth2\n  description: >-\n    OAuth 2.1 authorization-code flow with mandatory PKCE (S256) and public clients\n    (token_endpoint_auth_methods_supported = none), protecting the Model Context Protocol\n    endpoints. Client identity uses a client_id metadata document rather than dynamic\n\
  \    registration.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.redefinemeat.com/oauth/authorize\n    tokenUrl: https://www.redefinemeat.com/oauth/token\n    revocationUrl: https://www.redefinemeat.com/oauth/revoke\n    scopes: [mcp]\n  - flow: refreshToken\n    tokenUrl: https://www.redefinemeat.com/oauth/token\n  sources: [https://www.redefinemeat.com/.well-known/oauth-authorization-server]\n- name: wooCommerceKeys\n  type: apiKey\n  in: query\n  parameter: consumer_key / consumer_secret\n  status: inferred-not-verified\n  description: >-\n    The wc/v3, wc/v2 and wc/v1 namespaces are registered on this host (234 routes). WooCommerce\n    normally authenticates these with consumer key/secret pairs, but nothing on this host\n    documents or confirms that; an anonymous GET /wc/v3/products returned HTTP 401\n    {\"code\":\"woocommerce_rest_cannot_view\",\"message\":\"Sorry, you cannot list resources.\"}.\n    Recorded as inferred, not asserted.\n  sources:\
  \ [https://www.redefinemeat.com/wp-json/]\nx-evidence:\n  fetched: '2026-08-05'\n  probes:\n  - url: https://www.redefinemeat.com/wp-json/\n    http_status: 200\n  - url: https://www.redefinemeat.com/wp-json/wc/store/v1/products?per_page=2\n    http_status: 200\n  - url: https://www.redefinemeat.com/wp-json/wc/store/v1/cart/add-item/\n    http_status: 401\n  - url: https://www.redefinemeat.com/wp-json/wc/v3/products/\n    http_status: 401\n  - url: https://www.redefinemeat.com/.well-known/oauth-authorization-server\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redefine-meat/refs/heads/main/authentication/redefine-meat-authentication.yml
summary_line: apiKey/http/oauth2 · 7 schemes
tags:
- Food and Beverage
- Alternative Protein
- Plant-Based
- Food Technology
- Manufacturing
- E-Commerce
- WooCommerce
- WordPress
- Retail
- MCP
---
