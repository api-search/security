---
api_key_in:
- body
- path
- query
auth_types:
- apiKey
- custom-hmac-signature
description: ''
kind: authentication
layout: security
method: searched
name: Lucky Cart Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lucky Cart secures its APIs with apiKey and custom-hmac-signature across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lucky Cart
provider_slug: lucky-cart
scheme_count: 3
schemes:
- aliases:
  - AUTH_KEY
  - authKey
  - siteKey
  description: The per-site public identifier. It appears as the first path segment on the displayer and promo-matching hosts (/{siteKey}/{shopper}/banner/{subset}/{pageType}/{format}), as the siteKey query parameter on the Shopper Experience and Game Experience APIs, and as a body field on the Shopper Events API. Set with `new LuckyCart(AUTH_KEY, AUTH_SECRET)` in JavaScript, `LuckyCart.shared.setSiteKey("siteKeyToken")` in Swift, and `LCAuthorization(AUTH_KEY, "")` in Kotlin.
  in:
  - path
  - query
  - body
  name: siteKey
  sources:
  - luckycart-js-sdk/sdk/src/luckycart.js
  - lucky-cart-ios/Sources/LuckyCartSDK/LuckyCart.swift
  type: apiKey
- description: A shared secret used to sign write requests to the core API. It is never sent on the wire. The JS SDK signs the current UNIX timestamp with HMAC-SHA256 keyed by the secret (CryptoJS.HmacSHA256(ts, this.auth.secret)) and appends four fields to the request body — auth_ts (the timestamp), auth_key (the site key), auth_v ("2.0", the signature scheme version) and auth_sign (the hex digest). Only signed calls carry it; read calls to the banner, experience and game-data endpoints are unsigned. Note the Android SDK constructs LCAuthorization with an EMPTY secret (`LCAuthorization(AUTH_KEY, "")`), so the mobile surface appears to exercise only the unsigned read paths.
  in: body
  name: auth_secret
  scheme: hmac-sha256-request-signature
  signature:
    algorithm: HMAC-SHA256
    applies_to:
    - POST https://api.luckycart.com/cart/ticket
    fields:
    - auth_ts
    - auth_key
    - auth_v
    - auth_sign
    signed_payload: UNIX timestamp in seconds, as a string
    version_field: auth_v
    version_value: '2.0'
  sources:
  - luckycart-js-sdk/sdk/src/luckycart.js
  type: custom
- description: Not a credential, but required alongside the site key on nearly every call. The retailer's own customer identifier, set with setShopper()/setUser()/setUser(). The JS SDK README warns that an "automaton" must already be attached to the supplied shopperUid before cart data will be accepted, which means shopper identifiers are provisioned on the Lucky Cart side rather than accepted arbitrarily.
  in:
  - path
  - query
  - body
  name: shopperId
  type: identifier
slug: lucky-cart-authentication
source_filename: lucky-cart-authentication.yml
source_heading: Authentication Profile
source_url: https://github.com/lucky-cart/luckycart-js-sdk/blob/master/sdk/src/luckycart.js
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://github.com/lucky-cart/luckycart-js-sdk\nsources:\n- https://github.com/lucky-cart/luckycart-js-sdk/blob/master/sdk/src/luckycart.js\n- https://github.com/lucky-cart/luckycart-js-sdk#initialization\n- https://github.com/lucky-cart/lucky-cart-ios#configuration\n- https://github.com/lucky-cart/lucky-cart-android#use-in-client-application\nnote: >-\n  Lucky Cart publishes no OpenAPI, so nothing here is derived from a machine-readable\n  contract. Everything below is read from the authentication code and installation\n  instructions in Lucky Cart's own three first-party SDK repositories. Lucky Cart does\n  not use OAuth 2.0, OpenID Connect, or HTTP bearer tokens anywhere in the published\n  client surface. Credentials are issued out of band: the JS SDK README states the key\n  and secret are \"provided by our integration team\", so there is no self-service key\n  issuance. There is no public auth reference page — the Help\
  \ Centre at\n  kb.luckycart.com that would carry one is access-restricted (HTTP 403).\nsummary:\n  types:\n  - apiKey\n  - custom-hmac-signature\n  api_key_in:\n  - body\n  - path\n  - query\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\n  bearer_tokens: false\n  self_service_key_issuance: false\n  credential_issuance: manual, via the Lucky Cart integration team\nschemes:\n- name: siteKey\n  type: apiKey\n  aliases:\n  - AUTH_KEY\n  - authKey\n  - siteKey\n  in:\n  - path\n  - query\n  - body\n  description: >-\n    The per-site public identifier. It appears as the first path segment on the\n    displayer and promo-matching hosts\n    (/{siteKey}/{shopper}/banner/{subset}/{pageType}/{format}), as the siteKey query\n    parameter on the Shopper Experience and Game Experience APIs, and as a body field on\n    the Shopper Events API. Set with `new LuckyCart(AUTH_KEY, AUTH_SECRET)` in\n    JavaScript, `LuckyCart.shared.setSiteKey(\"siteKeyToken\")` in Swift, and\n    `LCAuthorization(AUTH_KEY,\
  \ \"\")` in Kotlin.\n  sources:\n  - luckycart-js-sdk/sdk/src/luckycart.js\n  - lucky-cart-ios/Sources/LuckyCartSDK/LuckyCart.swift\n- name: auth_secret\n  type: custom\n  scheme: hmac-sha256-request-signature\n  in: body\n  description: >-\n    A shared secret used to sign write requests to the core API. It is never sent on the\n    wire. The JS SDK signs the current UNIX timestamp with HMAC-SHA256 keyed by the\n    secret (CryptoJS.HmacSHA256(ts, this.auth.secret)) and appends four fields to the\n    request body — auth_ts (the timestamp), auth_key (the site key), auth_v (\"2.0\", the\n    signature scheme version) and auth_sign (the hex digest). Only signed calls carry\n    it; read calls to the banner, experience and game-data endpoints are unsigned. Note\n    the Android SDK constructs LCAuthorization with an EMPTY secret\n    (`LCAuthorization(AUTH_KEY, \"\")`), so the mobile surface appears to exercise only\n    the unsigned read paths.\n  signature:\n    algorithm: HMAC-SHA256\n\
  \    signed_payload: UNIX timestamp in seconds, as a string\n    version_field: auth_v\n    version_value: '2.0'\n    fields:\n    - auth_ts\n    - auth_key\n    - auth_v\n    - auth_sign\n    applies_to:\n    - POST https://api.luckycart.com/cart/ticket\n  sources:\n  - luckycart-js-sdk/sdk/src/luckycart.js\n- name: shopperId\n  type: identifier\n  in:\n  - path\n  - query\n  - body\n  description: >-\n    Not a credential, but required alongside the site key on nearly every call. The\n    retailer's own customer identifier, set with setShopper()/setUser()/setUser(). The\n    JS SDK README warns that an \"automaton\" must already be attached to the supplied\n    shopperUid before cart data will be accepted, which means shopper identifiers are\n    provisioned on the Lucky Cart side rather than accepted arbitrarily.\ntransport:\n  https_required: true\n  content_type: application/json\n  observed_headers:\n  - Content-Type: application/json\n  - Accept: application/json\n  note: >-\n \
  \   No Authorization header is used anywhere in the published SDKs. Credentials travel\n    as path segments, query parameters and body fields, which means the site key is\n    visible in URLs and therefore in browser history, referrers and intermediary logs.\n    This is consistent with the product design — the JS SDK is loaded into a retailer's\n    public storefront pages, so the site key is a public identifier by construction and\n    the secret is the only real credential.\ngaps:\n- no published authentication reference page (kb.luckycart.com returns 403)\n- no OpenAPI securitySchemes to validate this profile against\n- no documented key rotation, revocation or expiry policy\n- no scopes or permissions model — access is all-or-nothing per site key\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lucky-cart/refs/heads/main/authentication/lucky-cart-authentication.yml
summary_line: apiKey/custom-hmac-signature · 3 schemes
tags:
- Company
- Retail Media
- MarTech
- E-Commerce
- Advertising
- Personalization
- Loyalty
- CPG
- Grocery
- Promotions
- Gamification
- Shopper Marketing
- First-Party Data
- France
---
