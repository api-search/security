---
api_key_in: []
api_specs:
- filename: friendbuy-analytics-api-openapi.yml
  format: yaml
  label: Friendbuy Analytics API
  slug: friendbuy-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/friendbuy/refs/heads/main/openapi/friendbuy-analytics-api-openapi.yml
- filename: friendbuy-authorization-api-openapi.yml
  format: yaml
  label: Friendbuy Authorization API
  slug: friendbuy-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/friendbuy/refs/heads/main/openapi/friendbuy-authorization-api-openapi.yml
- filename: friendbuy-customers-api-openapi.yml
  format: yaml
  label: Friendbuy Customers API
  slug: friendbuy-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/friendbuy/refs/heads/main/openapi/friendbuy-customers-api-openapi.yml
- filename: friendbuy-events-api-openapi.yml
  format: yaml
  label: Friendbuy Events API
  slug: friendbuy-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/friendbuy/refs/heads/main/openapi/friendbuy-events-api-openapi.yml
- filename: friendbuy-management-api-openapi.yml
  format: yaml
  label: Friendbuy Management API
  slug: friendbuy-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/friendbuy/refs/heads/main/openapi/friendbuy-management-api-openapi.yml
- filename: friendbuy-referrals-api-openapi.yml
  format: yaml
  label: Friendbuy Referrals API
  slug: friendbuy-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/friendbuy/refs/heads/main/openapi/friendbuy-referrals-api-openapi.yml
- filename: friendbuy-rewards-loyalty-api-openapi.yml
  format: yaml
  label: Friendbuy Rewards & Loyalty API
  slug: friendbuy-rewards-loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/friendbuy/refs/heads/main/openapi/friendbuy-rewards-loyalty-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Friendbuy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Friendbuy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Friendbuy
provider_slug: friendbuy
scheme_count: 1
schemes:
- applied_to: every operation in every Friendbuy Merchant API spec
  bearerFormat: JWT
  description: 'Bearer JWT obtained from POST /authorization by exchanging your account key and secret. Passed as `Authorization: Bearer <token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/friendbuy-analytics-api-openapi.yml
  - openapi/friendbuy-authorization-api-openapi.yml
  - openapi/friendbuy-customers-api-openapi.yml
  - openapi/friendbuy-events-api-openapi.yml
  - openapi/friendbuy-management-api-openapi.yml
  - openapi/friendbuy-referrals-api-openapi.yml
  - openapi/friendbuy-rewards-loyalty-api-openapi.yml
  type: http
slug: friendbuy-authentication
source_filename: friendbuy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/ (7 refined specs in this repo)\ndocs: https://developers.friendbuy.com\nnote: >-\n  Upgraded from derived to searched on 2026-08-13 by reading the \"Authorization\"\n  and \"Authentication Scheme\" sections of the Friendbuy developer documentation.\n  The spec-derived baseline (a single http/bearer scheme) is correct but tells an\n  agent nothing about how to obtain the token, how long it lives, or how the\n  credential is issued — all three are recorded below from the docs. Friendbuy\n  runs NO OAuth 2.0 and NO OpenID Connect (there is no\n  /.well-known/openid-configuration and no oauth2 securityScheme anywhere), so\n  there is no scopes/ artifact for this provider.\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  bearer_formats: [JWT]\n  api_key_in: []\n  oauth2_flows: []\n  scopes: none\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Bearer JWT obtained\
  \ from POST /authorization by exchanging your account key and secret. Passed as `Authorization: Bearer <token>`.'\n  applied_to: every operation in every Friendbuy Merchant API spec\n  sources:\n  - openapi/friendbuy-analytics-api-openapi.yml\n  - openapi/friendbuy-authorization-api-openapi.yml\n  - openapi/friendbuy-customers-api-openapi.yml\n  - openapi/friendbuy-events-api-openapi.yml\n  - openapi/friendbuy-management-api-openapi.yml\n  - openapi/friendbuy-referrals-api-openapi.yml\n  - openapi/friendbuy-rewards-loyalty-api-openapi.yml\ntoken_exchange:\n  operation: createAuthorization\n  method: POST\n  url: https://mapi.fbot.me/v1/authorization\n  content_type: application/json\n  authentication: none (the key/secret pair IS the credential)\n  request:\n    key: Your Merchant API access key.\n    secret: Your Merchant API secret.\n  response:\n    tokenType: Bearer\n    token: The JWT to send on subsequent requests.\n    expires: ISO 8601 timestamp at which the token stops working.\n\
  \  lifetime: short-lived; the exact TTL is not published — read `expires` from the response\n  guidance: Cache the token until near `expires` and re-authorize; do not call /authorization per request.\ncredential_issuance:\n  self_serve: false\n  process: >-\n    Account key and secret are issued by Friendbuy. The documentation instructs\n    merchants to \"Contact Friendbuy support for your key and secret\"; keys are\n    surfaced in the Developer Center section of the Retailer App\n    (https://retailer.fbot.me). There is no developer sign-up that yields an API\n    credential, and no sandbox or test-mode key.\n  gate: paid plan (contact sales)\nother_credentials:\n- name: merchantId\n  surface: browser Merchant SDK\n  where: https://retailer.fbot.me/settings/general\n  description: >-\n    Public identifier pushed onto window.friendbuyAPI to load the merchant's\n    campaign bundle. Not a secret and not accepted by the Merchant API.\n- name: secret key (webhook signing)\n  surface: outbound\
  \ webhooks and callbacks\n  description: >-\n    The same merchant secret is used to compute the base64 HMAC-SHA256 signature\n    delivered in the X-Friendbuy-Hmac-SHA256 header. Verify it over the raw\n    request body before parsing. See asyncapi/friendbuy-webhooks.yml.\n- name: customer authentication signature\n  surface: browser Merchant SDK\n  description: >-\n    Merchant-signed identity handshake documented under \"Customer\n    Authentication\", used so widget state binds to a verified customer rather\n    than an anonymous visitor.\nunauthorized_response:\n  status: 401\n  envelope: '{error, message, code, reference}'\n  guidance: Re-run the token exchange and retry once; a repeated 401 means the key/secret pair is wrong or revoked.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/friendbuy/refs/heads/main/authentication/friendbuy-authentication.yml
summary_line: http · 1 scheme
tags:
- Referral Marketing
- Loyalty
- Rewards
- Ecommerce
- Marketing
- Advocacy
---
