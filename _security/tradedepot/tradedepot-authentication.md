---
api_key_in:
- sdk-initialization
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Tradedepot Authentication
name_suffix: Authentication
oauth_flows: []
overview: TradeDepot secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TradeDepot
provider_slug: tradedepot
scheme_count: 1
schemes:
- description: Partner API key passed to the ShopTopUp checkout SDK at initialization (co.tradedepot.shop.sdk.checkout.Checkout.initialize(context, apiKey)).
  name: shopCheckoutApiKey
  sources:
  - https://github.com/tradedepot/react-native-shop-checkout#readme
  - https://github.com/tradedepot/agent-checkout-sdk-android
  type: apiKey
slug: tradedepot-authentication
source_filename: tradedepot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://github.com/tradedepot/react-native-shop-checkout\ndocs: https://github.com/tradedepot/react-native-shop-checkout#readme\nnotes: >-\n  TradeDepot publishes no public REST API or developer portal, so there are no\n  OpenAPI securitySchemes to derive from. The only documented developer-facing\n  authentication is the API key used to initialize the ShopTopUp Agent/Shop\n  Checkout mobile SDKs (Android AAR, React Native, Cordova):\n  Checkout.initialize(this, \"API_KEY\"). Keys are issued by TradeDepot to\n  integration partners; there is no self-serve signup or key management surface.\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - sdk-initialization\n  oauth2_flows: []\nschemes:\n  - name: shopCheckoutApiKey\n    type: apiKey\n    description: >-\n      Partner API key passed to the ShopTopUp checkout SDK at initialization\n      (co.tradedepot.shop.sdk.checkout.Checkout.initialize(context, apiKey)).\n    sources:\n\
  \      - https://github.com/tradedepot/react-native-shop-checkout#readme\n      - https://github.com/tradedepot/agent-checkout-sdk-android\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tradedepot/refs/heads/main/authentication/tradedepot-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Applicative Saas
- B2B Commerce
- Retail Distribution
- FMCG
- Ecommerce
- Mobile SDKs
- Africa
- Nigeria
---
