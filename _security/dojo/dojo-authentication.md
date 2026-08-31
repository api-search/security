---
api_key_in:
- header
api_specs:
- filename: dojo-areas-api-openapi.yml
  format: yaml
  label: Dojo Areas API
  slug: dojo-areas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dojo/refs/heads/main/openapi/dojo-areas-api-openapi.yml
- filename: dojo-capabilities-api-openapi.yml
  format: yaml
  label: Dojo Capabilities API
  slug: dojo-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dojo/refs/heads/main/openapi/dojo-capabilities-api-openapi.yml
- filename: dojo-captures-api-openapi.yml
  format: yaml
  label: Dojo Captures API
  slug: dojo-captures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dojo/refs/heads/main/openapi/dojo-captures-api-openapi.yml
- filename: dojo-customers-api-openapi.yml
  format: yaml
  label: Dojo Customers API
  slug: dojo-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dojo/refs/heads/main/openapi/dojo-customers-api-openapi.yml
- filename: dojo-events-api-openapi.yml
  format: yaml
  label: Dojo Events API
  slug: dojo-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dojo/refs/heads/main/openapi/dojo-events-api-openapi.yml
- filename: dojo-flows-api-openapi.yml
  format: yaml
  label: Dojo Flows API
  slug: dojo-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dojo/refs/heads/main/openapi/dojo-flows-api-openapi.yml
- filename: dojo-orders-api-openapi.yml
  format: yaml
  label: Dojo Orders API
  slug: dojo-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dojo/refs/heads/main/openapi/dojo-orders-api-openapi.yml
- filename: dojo-parties-api-openapi.yml
  format: yaml
  label: Dojo Parties API
  slug: dojo-parties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dojo/refs/heads/main/openapi/dojo-parties-api-openapi.yml
- filename: dojo-payment-intents-api-openapi.yml
  format: yaml
  label: Dojo Payment intents API
  slug: dojo-payment-intents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dojo/refs/heads/main/openapi/dojo-payment-intents-api-openapi.yml
- filename: dojo-refunds-api-openapi.yml
  format: yaml
  label: Dojo Refunds API
  slug: dojo-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dojo/refs/heads/main/openapi/dojo-refunds-api-openapi.yml
- filename: dojo-reservations-api-openapi.yml
  format: yaml
  label: Dojo Reservations API
  slug: dojo-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dojo/refs/heads/main/openapi/dojo-reservations-api-openapi.yml
- filename: dojo-reversal-api-openapi.yml
  format: yaml
  label: Dojo Reversal API
  slug: dojo-reversal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dojo/refs/heads/main/openapi/dojo-reversal-api-openapi.yml
- filename: dojo-setup-intents-api-openapi.yml
  format: yaml
  label: Dojo Setup intents API
  slug: dojo-setup-intents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dojo/refs/heads/main/openapi/dojo-setup-intents-api-openapi.yml
- filename: dojo-tables-api-openapi.yml
  format: yaml
  label: Dojo Tables API
  slug: dojo-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dojo/refs/heads/main/openapi/dojo-tables-api-openapi.yml
- filename: dojo-tap-to-pay-on-iphone-api-openapi.yml
  format: yaml
  label: Dojo Tap to Pay on iPhone API
  slug: dojo-tap-to-pay-on-iphone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dojo/refs/heads/main/openapi/dojo-tap-to-pay-on-iphone-api-openapi.yml
- filename: dojo-terminal-sessions-api-openapi.yml
  format: yaml
  label: Dojo Terminal sessions API
  slug: dojo-terminal-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dojo/refs/heads/main/openapi/dojo-terminal-sessions-api-openapi.yml
- filename: dojo-terminals-api-openapi.yml
  format: yaml
  label: Dojo Terminals API
  slug: dojo-terminals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dojo/refs/heads/main/openapi/dojo-terminals-api-openapi.yml
- filename: dojo-transactions-api-openapi.yml
  format: yaml
  label: Dojo Transactions API
  slug: dojo-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dojo/refs/heads/main/openapi/dojo-transactions-api-openapi.yml
- filename: dojo-webhooks-api-openapi.yml
  format: yaml
  label: Dojo Webhooks API
  slug: dojo-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dojo/refs/heads/main/openapi/dojo-webhooks-api-openapi.yml
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
- Point-of-Sale
- Webhook
---
