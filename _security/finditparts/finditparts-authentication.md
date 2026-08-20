---
api_key_in: []
api_specs:
- filename: finditparts-reseller-api-openapi.yml
  format: yaml
  label: FinditParts Reseller API
  slug: finditparts-reseller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finditparts/refs/heads/main/openapi/finditparts-reseller-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Finditparts Authentication
name_suffix: Authentication
oauth_flows: []
overview: FinditParts secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: FinditParts
provider_slug: finditparts
scheme_count: 2
schemes:
- algorithm: HS256
  bearerFormat: JWT
  claims:
  - claim: iss
    description: The Reseller Client ID provided by FinditParts.
    required: true
  - claim: exp
    description: Expiration. FinditParts instructs that this be kept as short as reasonable to prevent requests from being replayed.
    required: true
  - claim: sub
    description: The Customer Reference. Required on endpoints that act on behalf of a specific customer (createResellerCustomerSession, shippingMethods, and productSearch when account-specific pricing is wanted). Omitting sub returns generic list pricing rather than account pricing.
    required: conditional
  - claim: data.intent
    description: Declares the purpose of the call. Documented values are PRODUCT_SEARCH, SHIPPING_METHODS, USER_SETUP and NEW_ORDER.
    required: conditional
  - claim: data
    description: On shippingMethods the JWT may carry the line_items/address payload inside data as an alternative to sending them as query parameters.
    required: conditional
  description: A separately generated, short-lived JWT for each request, signed with the Reseller Client Secret using HS256.
  header: 'Authorization: Bearer JWT.TOKEN.HERE'
  name: resellerJWT
  per_request: true
  scheme: bearer
  signing_key: Reseller Client Secret (provided by FinditParts)
  sources:
  - https://api-docs.finditparts.com/
  - openapi/finditparts-reseller-api-openapi.yml
  type: http
- bearerFormat: opaque-api-key
  description: An issued API key, for client-side apps that cannot hold a JWT signing secret — FinditParts names mobile apps and single-buyer partner applications. Issued to reseller clients alongside the JWT credentials.
  grants:
  - Non-user-specific endpoints — product search, create session, create user
  - The Partner surface (partnersShippingMethods, partnersPlaceOrder) requires a Partner API key
  - The Master Account surface (listResellerCustomers) requires a Master Account API key
  header: 'Authorization: Bearer api-XYZ123'
  key_prefix: api-
  key_shape: api-XYZ123
  name: apiKey
  restrictions: 'User-specific calls (user-specific pricing in product search, cart operations, order creation and order history) are not reachable with the API key alone. An API-key client must first exchange a user''s credentials for a user-specific JWT via createSession (that call itself still requires the API key), then present the returned user JWT as Authorization: Bearer USER.JWT.TOKEN.'
  scheme: bearer
  sources:
  - https://api-docs.finditparts.com/
  type: http
slug: finditparts-authentication
source_filename: finditparts-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://api-docs.finditparts.com/\ndocs: https://api-docs.finditparts.com/\nnote: >-\n  Upgraded from the mechanically derived profile using the authentication section\n  FinditParts publishes in the overview of its own \"FinditParts Reseller API 2.0.1\"\n  Postman documentation. FinditParts uses no OAuth 2.0 and no OpenID Connect — there\n  is no authorization server, no scope surface and no consent screen, so no\n  scopes/ artifact is emitted for this provider. Both credentials travel in the same\n  Authorization: Bearer header, which is why a purely spec-derived profile collapses\n  them into one http/bearer scheme; the two are distinct credential types with\n  distinct capability, and are recorded separately here.\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  bearer_formats:\n  - JWT\n  - opaque-api-key\n  oauth2_flows: []\n  api_key_in: []\n  credential_issuance: manual\n  credential_issuer: FinditParts\
  \ (Reseller Client ID + Reseller Client Secret, and an API key,\n    are issued by FinditParts to approved reseller/partner clients)\nschemes:\n- name: resellerJWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  algorithm: HS256\n  signing_key: Reseller Client Secret (provided by FinditParts)\n  header: 'Authorization: Bearer JWT.TOKEN.HERE'\n  per_request: true\n  description: >-\n    A separately generated, short-lived JWT for each request, signed with the\n    Reseller Client Secret using HS256.\n  claims:\n  - claim: iss\n    required: true\n    description: The Reseller Client ID provided by FinditParts.\n  - claim: exp\n    required: true\n    description: Expiration. FinditParts instructs that this be kept as short as reasonable\n      to prevent requests from being replayed.\n  - claim: sub\n    required: conditional\n    description: The Customer Reference. Required on endpoints that act on behalf of a\n      specific customer (createResellerCustomerSession, shippingMethods,\
  \ and productSearch\n      when account-specific pricing is wanted). Omitting sub returns generic list pricing\n      rather than account pricing.\n  - claim: data.intent\n    required: conditional\n    description: Declares the purpose of the call. Documented values are PRODUCT_SEARCH,\n      SHIPPING_METHODS, USER_SETUP and NEW_ORDER.\n  - claim: data\n    required: conditional\n    description: On shippingMethods the JWT may carry the line_items/address payload\n      inside data as an alternative to sending them as query parameters.\n  sources:\n  - https://api-docs.finditparts.com/\n  - openapi/finditparts-reseller-api-openapi.yml\n- name: apiKey\n  type: http\n  scheme: bearer\n  bearerFormat: opaque-api-key\n  key_prefix: api-\n  key_shape: api-XYZ123\n  header: 'Authorization: Bearer api-XYZ123'\n  description: >-\n    An issued API key, for client-side apps that cannot hold a JWT signing secret —\n    FinditParts names mobile apps and single-buyer partner applications. Issued\
  \ to\n    reseller clients alongside the JWT credentials.\n  grants:\n  - Non-user-specific endpoints — product search, create session, create user\n  - The Partner surface (partnersShippingMethods, partnersPlaceOrder) requires a Partner API key\n  - The Master Account surface (listResellerCustomers) requires a Master Account API key\n  restrictions: >-\n    User-specific calls (user-specific pricing in product search, cart operations,\n    order creation and order history) are not reachable with the API key alone. An\n    API-key client must first exchange a user's credentials for a user-specific JWT\n    via createSession (that call itself still requires the API key), then present\n    the returned user JWT as Authorization: Bearer USER.JWT.TOKEN.\n  sources:\n  - https://api-docs.finditparts.com/\ntoken_lifecycle:\n- token: reseller request JWT\n  ttl: per-request, issuer-chosen (docs instruct \"as short as reasonable\")\n  refresh: regenerate and sign a new token for every request\n\
  - token: user-specific session JWT\n  ttl: 1 month (default, per the createSession and refreshSession documentation)\n  refresh: refreshSession returns a new user-specific JWT; call it prior to expiration\n  revocation: destroySessions destroys the current sessions for the user\nalternate_credentials:\n- name: cart token\n  description: >-\n    Every cart operation documents \"Requires a user specific JWT in the Authorization\n    header or a cart token parameter\" — an anonymous cart-scoped credential passed as\n    a request parameter. FinditParts does not document the parameter name or issuance\n    in the public collection.\n  documented: partial\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finditparts/refs/heads/main/authentication/finditparts-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- E-Commerce
- Marketplace
- Automotive
- Parts
- Heavy Duty Trucking
- Fleet
- Logistics
- Commerce
- Catalog
- Order
- Shipping
---
