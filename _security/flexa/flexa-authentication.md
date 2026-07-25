---
api_key_in: []
api_specs:
- filename: flexa-assets-api-openapi.yml
  format: yaml
  label: Flexa Assets API
  slug: flexa-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexa/refs/heads/main/openapi/flexa-assets-api-openapi.yml
- filename: flexa-commerce-intents-api-openapi.yml
  format: yaml
  label: Flexa Commerce Intents API
  slug: flexa-commerce-intents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexa/refs/heads/main/openapi/flexa-commerce-intents-api-openapi.yml
- filename: flexa-events-api-openapi.yml
  format: yaml
  label: Flexa Events API
  slug: flexa-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexa/refs/heads/main/openapi/flexa-events-api-openapi.yml
- filename: flexa-refunds-api-openapi.yml
  format: yaml
  label: Flexa Refunds API
  slug: flexa-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexa/refs/heads/main/openapi/flexa-refunds-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Flexa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Flexa secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Flexa
provider_slug: flexa
scheme_count: 1
schemes:
- description: All requests to the Flexa API are authenticated with API keys using HTTP Basic Authentication. Include your API key as the "username" value in the Authorization header; a password is not required.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/flexa-openapi.json
  type: http
slug: flexa-authentication
source_filename: flexa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/flexa-openapi.json\ndocs: https://docs.flexa.co/api-reference/introduction\nsummary:\n  types:\n  - http\n  http_schemes:\n  - basic\n  api_key_delivery: HTTP Basic Authentication (API key as the username; no password required)\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: >-\n    All requests to the Flexa API are authenticated with API keys using HTTP\n    Basic Authentication. Include your API key as the \"username\" value in the\n    Authorization header; a password is not required.\n  sources:\n  - openapi/flexa-openapi.json\nkey_prefixes:\n- prefix: publishable_test_\n  mode: test\n  visibility: publishable\n- prefix: secret_test_\n  mode: test\n  visibility: secret\n- prefix: secret_live_\n  mode: live\n  visibility: secret\nnotes:\n- Test API keys (publishable_test_ / secret_test_) operate against test-mode assets including testnet assets and Flexa Credit (CR).\n- Live API keys (secret_live_)\
  \ only become functional once the business is approved to process payments.\n- API keys are provisioned by Flexa's Partnerships team after signup; rotation is handled via Flexa Support (support@flexa.co).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flexa/refs/heads/main/authentication/flexa-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Crypto
- Payments
- Digital Currency
- Cryptocurrency
- Fintech
- Blockchain
- Merchant Payments
- Web3
---
