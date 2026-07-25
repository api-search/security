---
api_key_in:
- header
api_specs:
- filename: dojo-api.json
  format: json
  label: Dojo API
  slug: dojo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dojo/refs/heads/main/openapi/dojo-api.json
- filename: dojo-transactions-api.json
  format: json
  label: Dojo Transaction API
  slug: dojo-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dojo/refs/heads/main/openapi/dojo-transactions-api.json
- filename: dojo-epos-data-api.json
  format: json
  label: Dojo EPOS Data API
  slug: dojo-epos-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dojo/refs/heads/main/openapi/dojo-epos-data-api.json
- filename: dojo-tap-to-pay-on-iphone-api.json
  format: json
  label: Dojo Tap to Pay on iPhone API
  slug: dojo-tap-to-pay-on-iphone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dojo/refs/heads/main/openapi/dojo-tap-to-pay-on-iphone-api.json
- filename: dojo-epos-tester-tool-api.json
  format: json
  label: Dojo EPOS Tester Tool API
  slug: dojo-epos-tester-tool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dojo/refs/heads/main/openapi/dojo-epos-tester-tool-api.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Dojo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dojo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dojo
provider_slug: dojo
scheme_count: 1
schemes:
- format: 'Authorization: Basic <api_key> (literal Basic prefix, not base64-encoded)'
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/dojo-api.json
  - openapi/dojo-tap-to-pay-on-iphone-api.json
  - openapi/dojo-transactions-api.json
  type: apiKey
slug: dojo-authentication
source_filename: dojo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: openapi/dojo-api.json + https://docs.dojo.tech/llms.txt\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/dojo-api.json\n  - openapi/dojo-tap-to-pay-on-iphone-api.json\n  - openapi/dojo-transactions-api.json\n  format: 'Authorization: Basic <api_key> (literal Basic prefix, not base64-encoded)'\ndocs: https://docs.dojo.tech/development-resources/api-keys\nnotes:\n- 'Auth is an API key sent as Authorization: Basic <api_key>; \"Basic \" is a literal prefix and the key\n  is NOT base64-encoded.'\n- Sandbox keys are prefixed sk_sandbox_ and production keys sk_prod_; the same host (api.dojo.tech) is\n  used for both and the key selects the environment.\n- Obtain keys from the Dojo Developer Portal (https://developer.dojo.tech).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dojo/refs/heads/main/authentication/dojo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Payments
- United Kingdom
- Payment Gateway
- Payment Processing
- Acquiring
- Card Payments
- In-Person Payments
- Terminals
- Point of Sale
- Webhooks
---
