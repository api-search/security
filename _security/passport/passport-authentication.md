---
api_key_in: []
api_specs:
- filename: passport-cart-api-openapi.yml
  format: yaml
  label: Passport Cart API
  slug: passport-cart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passport/refs/heads/main/openapi/passport-cart-api-openapi.yml
- filename: passport-healthcheck-api-openapi.yml
  format: yaml
  label: Passport Healthcheck API
  slug: passport-healthcheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passport/refs/heads/main/openapi/passport-healthcheck-api-openapi.yml
- filename: passport-order-api-openapi.yml
  format: yaml
  label: Passport Order API
  slug: passport-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passport/refs/heads/main/openapi/passport-order-api-openapi.yml
- filename: passport-product-price-api-openapi.yml
  format: yaml
  label: Passport Product Price API
  slug: passport-product-price-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passport/refs/heads/main/openapi/passport-product-price-api-openapi.yml
- filename: passport-rate-api-openapi.yml
  format: yaml
  label: Passport Rate API
  slug: passport-rate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passport/refs/heads/main/openapi/passport-rate-api-openapi.yml
- filename: passport-ship-api-openapi.yml
  format: yaml
  label: Passport Ship API
  slug: passport-ship-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passport/refs/heads/main/openapi/passport-ship-api-openapi.yml
- filename: passport-tax-and-duty-api-openapi.yml
  format: yaml
  label: Passport Tax And Duty API
  slug: passport-tax-and-duty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passport/refs/heads/main/openapi/passport-tax-and-duty-api-openapi.yml
- filename: passport-void-api-openapi.yml
  format: yaml
  label: Passport Void API
  slug: passport-void-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passport/refs/heads/main/openapi/passport-void-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Passport Authentication
name_suffix: Authentication
oauth_flows: []
overview: Passport declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Passport
provider_slug: passport
scheme_count: 1
schemes:
- applies_to: all operations
  description: '"Authentication and identification is done by providing an API key on every request as a custom HTTP header ''X-Access-Token''." — Passport Global API v3.15 documentation preamble.'
  id: api_key_header
  in: header
  issuance: '"During the onboarding or integration process, our Onboarding team will create an account for your organization and provide the API key to your designated point of contact, which is typically a member of the operations, development team, or one of the founders."'
  name: X-Access-Token
  required: true
  rotation_documented: false
  self_service: false
  type: apiKey
slug: passport-authentication
source_filename: passport-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://docs.passportglobal.com/ (Getting Started with Passport Global API, v3.15 — info.description)\ndocs: https://docs.passportglobal.com/\nsummary: >-\n  Passport Global API authentication is a single static API key sent on every request in a custom HTTP header,\n  X-Access-Token. Keys are not self-service: they are provisioned by the Passport onboarding team and handed to a\n  named point of contact at the brand during integration. There is no OAuth 2.0, no OpenID Connect, no mutual TLS,\n  and no scope model published on the public surface.\nschemes:\n- id: api_key_header\n  type: apiKey\n  in: header\n  name: X-Access-Token\n  required: true\n  applies_to: all operations\n  description: >-\n    \"Authentication and identification is done by providing an API key on every request as a custom HTTP header\n    'X-Access-Token'.\" — Passport Global API v3.15 documentation preamble.\n  issuance: >-\n    \"During the onboarding\
  \ or integration process, our Onboarding team will create an account for your organization\n    and provide the API key to your designated point of contact, which is typically a member of the operations,\n    development team, or one of the founders.\"\n  self_service: false\n  rotation_documented: false\ntransport:\n  https_required: true\n  note: \"Passport Global API is a REST-like API. All methods must be called using HTTPS.\"\nenvironments:\n- name: production\n  base_url: https://api.passportshipping.com/v3\n  key_scope: separate production key issued at onboarding\n- name: testing\n  base_url: https://api-stg.passportshipping.com/v3\n  key_scope: separate testing key issued at onboarding\nspec_gap:\n  securitySchemes_declared: false\n  note: >-\n    The published OpenAPI 3.0.1 document declares no components.securitySchemes and no security requirement on any\n    operation, even though every operation is key-gated in production. The auth model is described only in prose in\n   \
  \ info.description. This is captured as an enhancement in overlays/passport-public-api-overlay.yaml and is a\n    concrete fix for Passport to make in its own spec.\nobserved_behavior:\n- probe: GET https://api.passportshipping.com/v3/ping (no credentials)\n  http_status: 401\n  www_authenticate: Basic realm=Authorization Required\n  body: 'Unable to access the requested resource, authorization failed.'\n  fetched: '2026-08-04'\n- probe: GET https://api-stg.passportshipping.com/v3/ping (no credentials)\n  http_status: 401\n  body: 'Unable to access the requested resource, authorization failed.'\n  fetched: '2026-08-04'\nerror_responses:\n  '401':\n    message: Unable to access the requested resource, authorization failed.\n    details: missing/incorrect authorization data\n  '403':\n    message: Brand is blocked\ncross_links:\n  conventions: conventions/passport-conventions.yml\n  errors: errors/passport-problem-types.yml\n  sandbox: sandbox/passport-sandbox.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/passport/refs/heads/main/authentication/passport-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Shipping
- Logistics
- Cross-border eCommerce
- International Shipping
- Customs Compliance
- Landed Cost
- duties-and-taxes
- Parcel Delivery
- E-Commerce
- Merchant of Record
- Trade Compliance
---
