---
api_key_in: []
api_specs:
- filename: ciloo-cart-api-openapi.yml
  format: yaml
  label: Ciloo Cart API
  slug: ciloo-cart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ciloo/refs/heads/main/openapi/ciloo-cart-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Ciloo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ciloo secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ciloo
provider_slug: ciloo
scheme_count: 2
schemes:
- applies_to:
  - getCartItems
  - addCartItem
  - updateCartItem
  - removeCartItem
  - generateCustomerKeys
  - generateLoginToken
  - createCustomer
  - updateCustomer
  description: 'OAuth 1.0a with HMAC-SHA1. Required parameters: oauth_consumer_key, oauth_signature_method, oauth_timestamp, oauth_nonce, oauth_version, oauth_signature. Content-Type must be application/x-www-form-urlencoded on the ciloo/v1 namespace — a JSON content type causes signature failures. Body parameters are merged into the signature base string for POST and PUT only; path parameters (such as asset_id) are included. Signing key is urlencode(consumer_secret) + "&" — there is no token secret, so this is the two-legged variant.'
  in: Authorization header
  name: oauth1a
  scheme: OAuth
  signature_method: HMAC-SHA1
  sources:
  - openapi/ciloo-cart-api-openapi.yml
  spec: RFC 5849
  type: http
- applies_to:
  - generateCustomerLoginToken
  description: HTTP Basic authentication using the consumer key as username and consumer secret as password. The provider flags this as a deliberate exception to the OAuth rule.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/ciloo-cart-api-openapi.yml
  type: http
slug: ciloo-authentication
source_filename: ciloo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: openapi/ciloo-cart-api-openapi.yml\ndocs: https://api.cilooprint.com/ciloo-cart-api-documentation/#authentication-setup\nsummary:\n  types:\n  - http\n  http_schemes:\n  - OAuth\n  - basic\n  oauth_version: 1.0a\n  oauth2_flows: []\n  api_key_in: []\n  note: >-\n    Ciloo authenticates with OAuth 1.0a (HMAC-SHA1), not OAuth 2.0. There is no authorization server, no\n    scope surface, no OIDC discovery document and no bearer-token endpoint. One endpoint —\n    generateCustomerLoginToken — uses HTTP Basic instead.\nschemes:\n- name: oauth1a\n  type: http\n  scheme: OAuth\n  spec: RFC 5849\n  signature_method: HMAC-SHA1\n  in: Authorization header\n  description: >-\n    OAuth 1.0a with HMAC-SHA1. Required parameters: oauth_consumer_key, oauth_signature_method,\n    oauth_timestamp, oauth_nonce, oauth_version, oauth_signature. Content-Type must be\n    application/x-www-form-urlencoded on the ciloo/v1 namespace — a JSON content\
  \ type causes signature\n    failures. Body parameters are merged into the signature base string for POST and PUT only; path\n    parameters (such as asset_id) are included. Signing key is urlencode(consumer_secret) + \"&\" — there\n    is no token secret, so this is the two-legged variant.\n  sources:\n  - openapi/ciloo-cart-api-openapi.yml\n  applies_to:\n  - getCartItems\n  - addCartItem\n  - updateCartItem\n  - removeCartItem\n  - generateCustomerKeys\n  - generateLoginToken\n  - createCustomer\n  - updateCustomer\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic authentication using the consumer key as username and consumer secret as password. The\n    provider flags this as a deliberate exception to the OAuth rule.\n  sources:\n  - openapi/ciloo-cart-api-openapi.yml\n  applies_to:\n  - generateCustomerLoginToken\ncredential_tiers:\n- name: admin\n  prefixes: [ck_admin_, cs_admin_]\n  issued_by: Ciloo\n  purpose: Generating per-customer OAuth keys.\
  \ The provider states these should not be used for cart operations.\n- name: customer\n  prefixes: [ck_, cs_]\n  issued_by: POST /wp-json/ciloo/v1/generate_customer_keys\n  purpose: All cart operations, scoped to a single customer account.\n  delivery: >-\n    Keys are POSTed to a callback_url supplied on the request; return_keys=1 additionally returns them\n    in the response body.\nsession_tokens:\n  mechanism: auto-login token\n  issued_by: [generateLoginToken, generateCustomerLoginToken]\n  ttl_seconds: 3600\n  bound_to: customer + ip_address\n  transport: query string — {base_url}?action=autologin&token=<token>&path=/cart\nweaknesses_documented_by_provider:\n- >-\n  oauth_timestamp and oauth_nonce are accepted without validation, so OAuth 1.0a replay protection is\n  not enforced by the implementation.\n- >-\n  Session tokens travel in a URL query string, which is exposed to browser history, referrers and\n  intermediate logs.\n- Newly minted customer credentials are delivered over\
  \ an integrator-supplied callback URL.\nmissing:\n- No OAuth 2.0 or OpenID Connect surface (no scopes artifact is emitted — there are no scopes).\n- No mTLS, no signed requests on the printer callbacks, no key-rotation API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ciloo/refs/heads/main/authentication/ciloo-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Printing
- Branded Merchandise
- Promotional Products
- Print On Demand
- eCommerce
- Digital Asset Management
- Procurement
- Fulfillment
- Marketing
---
