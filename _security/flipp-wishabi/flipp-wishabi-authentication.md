---
api_key_in:
- query
api_specs:
- filename: flipp-wishabi-copyright-api-openapi.yml
  format: yaml
  label: Flipp (Wishabi) Copyright API
  slug: flipp-wishabi-copyright-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipp-wishabi/refs/heads/main/openapi/flipp-wishabi-copyright-api-openapi.yml
- filename: flipp-wishabi-fsa-api-openapi.yml
  format: yaml
  label: Flipp (Wishabi) Fsa API
  slug: flipp-wishabi-fsa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipp-wishabi/refs/heads/main/openapi/flipp-wishabi-fsa-api-openapi.yml
- filename: flipp-wishabi-products-api-openapi.yml
  format: yaml
  label: Flipp (Wishabi) Products API
  slug: flipp-wishabi-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipp-wishabi/refs/heads/main/openapi/flipp-wishabi-products-api-openapi.yml
- filename: flipp-wishabi-publications-api-openapi.yml
  format: yaml
  label: Flipp (Wishabi) Publications API
  slug: flipp-wishabi-publications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipp-wishabi/refs/heads/main/openapi/flipp-wishabi-publications-api-openapi.yml
- filename: flipp-wishabi-stores-api-openapi.yml
  format: yaml
  label: Flipp (Wishabi) Stores API
  slug: flipp-wishabi-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipp-wishabi/refs/heads/main/openapi/flipp-wishabi-stores-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Flipp Wishabi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Flipp (Wishabi) secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Flipp (Wishabi)
provider_slug: flipp-wishabi
scheme_count: 1
schemes:
- applies_to: Every FlyerKit v4.0 operation except GET /copyright, which is unauthenticated.
  description: '"Contact your Flipp technical contact for your API access token." Tokens are issued out of band by a Flipp account/technical contact - there is no self-service signup, no developer console, and no token endpoint. Tokens are passed to the FlyerKit API as URL query parameters.'
  in: query
  name: access_token
  parameter: access_token
  required: true
  sources:
  - openapi/flipp-wishabi-flyerkit-openapi.yml
  - https://api.flipp.com/flyerkit/v4.0/documentation
  type: apiKey
slug: flipp-wishabi-authentication
source_filename: flipp-wishabi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://api.flipp.com/flyerkit/v4.0/documentation\ndocs: https://api.flipp.com/flyerkit/v3.0/documentation\nnote: >-\n  The published FlyerKit Swagger 2.0 document declares NO `securityDefinitions` block -\n  authorization is expressed as a required `access_token` query parameter on every\n  operation except GET /copyright. `derive-authentication.py` therefore finds nothing to\n  aggregate; this profile is written from the provider's own published documentation,\n  which states the mechanism explicitly.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  oauth2_flows: []\n  self_service: false\nschemes:\n- name: access_token\n  type: apiKey\n  in: query\n  parameter: access_token\n  required: true\n  sources:\n  - openapi/flipp-wishabi-flyerkit-openapi.yml\n  - https://api.flipp.com/flyerkit/v4.0/documentation\n  description: >-\n    \"Contact your Flipp technical contact for your API access token.\" Tokens are issued\n\
  \    out of band by a Flipp account/technical contact - there is no self-service signup,\n    no developer console, and no token endpoint. Tokens are passed to the FlyerKit API as\n    URL query parameters.\n  applies_to: >-\n    Every FlyerKit v4.0 operation except GET /copyright, which is unauthenticated.\nissuance:\n  self_service: false\n  channel: Flipp technical contact / account manager\n  quoted: >-\n    \"Access tokens are issued by your Flipp technical contact and if needed, multiple\n    access tokens can be created for your various development teams or partners. Access\n    tokens should always be kept secret and not shared.\"\n  source: https://api.flipp.com/flyerkit/v4.0/documentation\npermissions:\n  model: per-token scoping\n  note: >-\n    v4.0 introduced a multi-token model: \"Updated the access token model, allowing\n    retailers to have multiple FlyerKit access tokens with different levels of\n    permission.\" One named permission is documented - viewing future (not\
  \ yet live)\n    publications and products via `see_future`, which \"requires an access token with\n    special permissions issued by your Flipp technical contact.\" Flipp publishes no\n    enumerated scope list, so there is no scopes/ artifact for this provider.\n  breaking_change: >-\n    \"access tokens from previous FlyerKit versions will no longer work in v4.0 and new\n    ones will need to be issued by your Flipp technical contact.\"\ntransport:\n  https_only: true\n  cors: true\n  cors_note: >-\n    \"The API allows cross-origin requests using CORS.\" (FlyerKit v2.0 and v3.0\n    documentation.) Because the token travels in the query string of a browser-visible\n    URL, a CORS-enabled front-end integration exposes it to the client.\nobservations:\n- >-\n  Credential in the query string, not a header. Query parameters are logged by\n  intermediaries, proxies and browser history; Flipp's own v3.0 docs temper this by\n  stating the token \"is not intended as a security mechanism ...\
  \ All data available\n  through the API is publicly available information.\"\n- No OAuth 2.0, no OpenID Connect, no mTLS, and no key-rotation endpoint is published.\n- >-\n  The mobile SDKs (FlyerKit iOS/Android, DVM) use a separate `clientToken` / SDK key,\n  also issued by Flipp; see components/flipp-wishabi-components.yml.\ncross_links:\n  conventions: conventions/flipp-wishabi-conventions.yml\n  errors: errors/flipp-wishabi-problem-types.yml\n  lifecycle: lifecycle/flipp-wishabi-lifecycle.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flipp-wishabi/refs/heads/main/authentication/flipp-wishabi-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Retail
- Retail Media
- Advertising
- Flyers
- Coupons
- E-Commerce
- Shopping
- Marketing
- Digital Circulars
- Publications
- Merchandising
- Product Data
- Store Locator
---
