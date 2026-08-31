---
api_key_in: []
auth_types: []
description: Authentication profile for the Yeeld Surcharging API, read from Yeeld's public integration guides. Yeeld publishes no OpenAPI, so no securityScheme could be derived; everything below is stated in prose on the pages cited and nothing is inferred. The full parameter-level reference is gated — theyeeld.com/products/surcharging-api answers "Is there a sandbox or API docs? Yes. Contact us to get access."
kind: authentication
layout: security
method: searched
name: Yeeld Authentication
name_suffix: Authentication
oauth_flows: []
overview: Yeeld declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Yeeld
provider_slug: yeeld
scheme_count: 2
schemes:
- description: Yeeld issues an API key per account. The merchant guide says "Yeeld applies the surcharging rules associated with your primary API key", so the key is both the credential and the tenant selector in the single-merchant model. The transport (header name vs. bearer scheme) is not published.
  evidence:
  - quote: 'Yeeld Configuration: You do not need to pass an account header. Yeeld applies the surcharging rules associated with your primary API key.'
    status: 200
    url: https://docs.theyeeld.com/integrations
  id: yeeld-api-key
  in: unknown
  name: unknown
  published_scheme_details: false
  type: apiKey
- description: Tenant-scoping header, REQUIRED for the Platforms & Marketplaces model. A platform calling on behalf of a sub-merchant passes that sub-merchant's Yeeld account ID so the surcharge is calculated against that merchant's location and settings. Not an authentication credential on its own — it rides alongside the platform's API key.
  evidence:
  - quote: You must provide the Yeeld-Account header in every API call to ensure the surcharge is calculated based on that specific sub-merchant's location and settings.
    status: 200
    url: https://docs.theyeeld.com/integrations
  - quote: you pass the sub-merchant's Yeeld account ID in the request header so Yeeld applies the correct rules for that merchant
    status: 200
    url: https://docs.theyeeld.com/integrations/platforms-and-marketplaces
  id: yeeld-account-header
  in: header
  name: Yeeld-Account
  type: apiKey
slug: yeeld-authentication
source_filename: yeeld-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Yeeld\nproviderId: yeeld\ngenerated: '2026-08-28'\nmethod: searched\nsource: >-\n  https://docs.theyeeld.com/integrations,\n  https://docs.theyeeld.com/integrations/merchant,\n  https://docs.theyeeld.com/integrations/platforms-and-marketplaces\ndescription: >-\n  Authentication profile for the Yeeld Surcharging API, read from Yeeld's public\n  integration guides. Yeeld publishes no OpenAPI, so no securityScheme could be derived;\n  everything below is stated in prose on the pages cited and nothing is inferred.\n  The full parameter-level reference is gated — theyeeld.com/products/surcharging-api\n  answers \"Is there a sandbox or API docs? Yes. Contact us to get access.\"\nschemes:\n  - id: yeeld-api-key\n    type: apiKey\n    in: unknown\n    name: unknown\n    description: >-\n      Yeeld issues an API key per account. The merchant guide says \"Yeeld applies the\n      surcharging rules associated\
  \ with your primary API key\", so the key is both the\n      credential and the tenant selector in the single-merchant model. The transport\n      (header name vs. bearer scheme) is not published.\n    evidence:\n      - url: https://docs.theyeeld.com/integrations\n        quote: >-\n          Yeeld Configuration: You do not need to pass an account header. Yeeld applies\n          the surcharging rules associated with your primary API key.\n        status: 200\n    published_scheme_details: false\n  - id: yeeld-account-header\n    type: apiKey\n    in: header\n    name: Yeeld-Account\n    description: >-\n      Tenant-scoping header, REQUIRED for the Platforms & Marketplaces model. A platform\n      calling on behalf of a sub-merchant passes that sub-merchant's Yeeld account ID so\n      the surcharge is calculated against that merchant's location and settings. Not an\n      authentication credential on its own — it rides alongside the platform's API key.\n    evidence:\n      - url: https://docs.theyeeld.com/integrations\n\
  \        quote: >-\n          You must provide the Yeeld-Account header in every API call to ensure the\n          surcharge is calculated based on that specific sub-merchant's location and settings.\n        status: 200\n      - url: https://docs.theyeeld.com/integrations/platforms-and-marketplaces\n        quote: >-\n          you pass the sub-merchant's Yeeld account ID in the request header so Yeeld\n          applies the correct rules for that merchant\n        status: 200\noauth2: false\nopenid_connect: false\nmutual_tls: false\nnotes:\n  - >-\n    Adjacent-but-not-Yeeld: the same guides tell you to hold \"a standard Stripe Secret Key\"\n    for your PSP. That is a Stripe credential used against Stripe, not a Yeeld auth scheme,\n    and is recorded here only so a reader does not confuse the two key types.\n  - >-\n    No /.well-known/oauth-authorization-server, /.well-known/oauth-protected-resource or\n    /.well-known/openid-configuration is served on any Yeeld host (all 404 on\
  \ 2026-08-28,\n    see well-known/yeeld-well-known.yml), which is consistent with a plain API-key model.\ngaps:\n  - Header or scheme name that carries the API key is not published.\n  - Key prefix / test-vs-live key distinction is not published.\n  - No key rotation, expiry, or scoping policy is published.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yeeld/refs/heads/main/authentication/yeeld-authentication.yml
summary_line: 2 schemes
tags:
- Payments
- Surcharging
- Credit Cards
- Compliance
- Stripe
- Checkout
- Fintech
- Payment Consulting
---
