---
anonymous_access: true
api_key_in: []
auth_types: []
description: There is no developer authentication programme. No API keys, no OAuth, no developer signup, no documented auth page anywhere on either the Korean parent site or the North American storefront. What exists is a WordPress/WooCommerce installation whose read surfaces answer anonymously and whose write and admin surfaces are refused with the platform's own session check.
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Abiomaterials Authentication
name_suffix: Authentication
oauth_flows: []
overview: A-Bio Materials declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: A-Bio Materials
provider_slug: abiomaterials
scheme_count: 3
schemes:
- applies_to:
  - GET /wp-json/wc/store/v1/products
  - GET /wp-json/wc/store/v1/products/categories
  - GET /wp-json/wp/v2/posts
  - GET /wp-json/g99-webmcp/v1/manifest
  - POST /wp-json/g99-webmcp/v1/execute
  - GET /wp-json/.well-known/api-catalog
  evidence: All returned HTTP 200 with real bodies to requests carrying no credentials of any kind, on 2026-09-06.
  id: none-anonymous
  type: none
- applies_to:
  - POST /wp-json/mcp/mcp-adapter-default-server
  - GET /wp-json/wp-abilities/v1/abilities
  - PATCH /wp-json/wp/v2/settings
  description: WordPress' own logged-in cookie plus a nonce. Unauthenticated calls are refused with HTTP 401 {"code":"rest_forbidden","message":"Sorry, you are not allowed to do that.","data":{"status":401}} and NO WWW-Authenticate header, so there is no discoverable challenge for an agent to follow.
  header: X-WP-Nonce
  id: wordpress-session
  nonce_endpoint: https://a-biousa.com/wp-json/g99-webmcp/v1/nonce
  nonce_evidence: GET returned HTTP 200 {"nonce":"...","expires":"<ISO8601>","header":"X-WP-Nonce"} anonymously; the nonce it issues is a visitor nonce, not a credential.
  type: cookie+nonce
- description: A B2B customer account login for the storefront. It is a human commerce login, not a developer or API credential; there is no token issuance, no key management page and no scope model behind it.
  id: customer-account
  type: human-login
  url: https://a-biousa.com/user-login/
slug: abiomaterials-authentication
source_filename: abiomaterials-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: >-\n  Live unauthenticated requests against every public surface on\n  https://a-biousa.com/wp-json/. No OpenAPI securitySchemes exist to derive\n  from - the provider publishes no specification - so every statement here is\n  an observed response, not a documented claim.\nname: Abiomaterials authentication profile\ndescription: >-\n  There is no developer authentication programme. No API keys, no OAuth, no\n  developer signup, no documented auth page anywhere on either the Korean parent\n  site or the North American storefront. What exists is a WordPress/WooCommerce\n  installation whose read surfaces answer anonymously and whose write and admin\n  surfaces are refused with the platform's own session check.\ndocumented: false\ndocs: null\nschemes:\n- id: none-anonymous\n  type: none\n  applies_to:\n  - GET /wp-json/wc/store/v1/products\n  - GET /wp-json/wc/store/v1/products/categories\n  - GET /wp-json/wp/v2/posts\n  - GET /wp-json/g99-webmcp/v1/manifest\n\
  \  - POST /wp-json/g99-webmcp/v1/execute\n  - GET /wp-json/.well-known/api-catalog\n  evidence: >-\n    All returned HTTP 200 with real bodies to requests carrying no credentials\n    of any kind, on 2026-09-06.\n- id: wordpress-session\n  type: cookie+nonce\n  header: X-WP-Nonce\n  applies_to:\n  - POST /wp-json/mcp/mcp-adapter-default-server\n  - GET /wp-json/wp-abilities/v1/abilities\n  - PATCH /wp-json/wp/v2/settings\n  description: >-\n    WordPress' own logged-in cookie plus a nonce. Unauthenticated calls are\n    refused with HTTP 401 {\"code\":\"rest_forbidden\",\"message\":\"Sorry, you are not\n    allowed to do that.\",\"data\":{\"status\":401}} and NO WWW-Authenticate header,\n    so there is no discoverable challenge for an agent to follow.\n  nonce_endpoint: https://a-biousa.com/wp-json/g99-webmcp/v1/nonce\n  nonce_evidence: >-\n    GET returned HTTP 200 {\"nonce\":\"...\",\"expires\":\"<ISO8601>\",\"header\":\"X-WP-Nonce\"}\n    anonymously; the nonce it issues is a visitor\
  \ nonce, not a credential.\n- id: customer-account\n  type: human-login\n  url: https://a-biousa.com/user-login/\n  description: >-\n    A B2B customer account login for the storefront. It is a human commerce\n    login, not a developer or API credential; there is no token issuance,\n    no key management page and no scope model behind it.\noauth: false\nopenid_connect: false\nmutual_tls: false\napi_keys: false\ngaps:\n- No authentication documentation is published on any host.\n- >-\n  The gated MCP endpoint returns 401 with no WWW-Authenticate header, so an\n  agent cannot discover how to authenticate even in principle.\nevidence:\n- url: https://a-biousa.com/wp-json/wc/store/v1/products?per_page=2\n  status: 200\n- url: https://a-biousa.com/wp-json/mcp/mcp-adapter-default-server\n  status: 401\n- url: https://a-biousa.com/wp-json/wp-abilities/v1/abilities\n  status: 401\n- url: https://a-biousa.com/wp-json/g99-webmcp/v1/nonce\n  status: 200\n- url: https://a-biousa.com/user-login/\n\
  \  status: 200\nchecked: '2026-09-06'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abiomaterials/refs/heads/main/authentication/abiomaterials-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Biomaterials
- Life Sciences
- Cosmetics
- Medical Devices
- Exosomes
- Manufacturing
- E-Commerce
- South Korea
---
