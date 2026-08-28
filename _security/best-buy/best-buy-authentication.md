---
api_key_in:
- query
api_specs:
- filename: best-buy-products-api-openapi.yml
  format: yaml
  label: Best Buy Products API
  slug: best-buy-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/openapi/best-buy-products-api-openapi.yml
- filename: best-buy-recommendations-api-openapi.yml
  format: yaml
  label: Best Buy Recommendations API
  slug: best-buy-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/openapi/best-buy-recommendations-api-openapi.yml
- filename: best-buy-stores-api-openapi.yml
  format: yaml
  label: Best Buy Stores API
  slug: best-buy-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/openapi/best-buy-stores-api-openapi.yml
auth_types:
- apiKey
description: Best Buy uses a single unscoped API key passed as a QUERY-STRING parameter (apiKey=) on every request. There is no OAuth, no OIDC, no bearer token, no signing, no key rotation endpoint and no scope model — one key grants everything the tier allows. The Commerce API uses a second, separately-issued key ("CAPI key") obtained by contacting Best Buy directly.
kind: authentication
layout: security
method: searched
name: Best Buy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Best Buy secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Best Buy
provider_slug: best-buy
scheme_count: 2
schemes:
- description: API key obtained by registering at developer.bestbuy.com and activating via email.
  example_form: https://api.bestbuy.com/v1/products?apiKey=YourAPIKey&format=json
  in: query
  name: apiKey
  parameter: apiKey
  sources:
  - openapi/best-buy-products-api-openapi.yml
  - openapi/best-buy-recommendations-api-openapi.yml
  - openapi/best-buy-stores-api-openapi.yml
  - https://bestbuyapis.github.io/api-documentation/#user-guide
  type: apiKey
- description: Separate key for the Commerce API, not issued by self-serve registration. Requested via developer.bestbuy.com/contact-us?topic=commerce-api; the Commerce API's full documentation is supplied only after the key is granted, so its exact auth mechanics are not public.
  gated: true
  in: query
  name: capiKey
  parameter: apiKey
  sources:
  - https://bestbuyapis.github.io/api-documentation/#commerce-api
  type: apiKey
slug: best-buy-authentication
source_filename: best-buy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://bestbuyapis.github.io/api-documentation/#user-guide + https://developer.bestbuy.com/ + openapi/\ndescription: >-\n  Best Buy uses a single unscoped API key passed as a QUERY-STRING parameter (apiKey=) on\n  every request. There is no OAuth, no OIDC, no bearer token, no signing, no key rotation\n  endpoint and no scope model — one key grants everything the tier allows. The Commerce API\n  uses a second, separately-issued key (\"CAPI key\") obtained by contacting Best Buy directly.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  oauth2: false\n  openid_connect: false\n  mtls: false\n  scoped: false\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: API key obtained by registering at developer.bestbuy.com and activating via email.\n  example_form: https://api.bestbuy.com/v1/products?apiKey=YourAPIKey&format=json\n  sources:\n  - openapi/best-buy-products-api-openapi.yml\n\
  \  - openapi/best-buy-recommendations-api-openapi.yml\n  - openapi/best-buy-stores-api-openapi.yml\n  - https://bestbuyapis.github.io/api-documentation/#user-guide\n- name: capiKey\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: >-\n    Separate key for the Commerce API, not issued by self-serve registration. Requested via\n    developer.bestbuy.com/contact-us?topic=commerce-api; the Commerce API's full documentation\n    is supplied only after the key is granted, so its exact auth mechanics are not public.\n  gated: true\n  sources:\n  - https://bestbuyapis.github.io/api-documentation/#commerce-api\ndocs: https://bestbuyapis.github.io/api-documentation/#user-guide\nsignup: https://developer.bestbuy.com\nfailure_modes:\n- status: 403\n  meaning: >-\n    Overloaded. Returned both for a missing/invalid API key AND for an exceeded call limit —\n    the two are not distinguishable from the response. Anonymous requests to any path on\n    api.bestbuy.com return {\"errorCode\"\
  :\"403\",\"errorMessage\":\"We were unable to locate your API Key.\"}\nagent_notes:\n- A key in the query string is logged by every proxy, CDN and browser history in the path. Agents should treat a Best Buy key as exposed-by-design and scope its blast radius accordingly — though with no scope model there is nothing to scope.\n- No documented rotation, expiry or revocation flow. Key lifecycle is manual, through the portal.\n- The OpenAPI declares the scheme as `apiKey` in `query`, and it is applied globally via a root-level `security:` block on all three specs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/authentication/best-buy-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Fortune 100
- Retail
- Consumer Electronics
- E-Commerce
- Product
- Stores
---
