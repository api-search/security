---
api_key_in:
- header
api_specs:
- filename: smartrr-openapi.yml
  format: yaml
  label: Smartrr Subscriptions API
  slug: smartrr-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartrr/refs/heads/main/openapi/smartrr-openapi.yml
- filename: smartrr-openapi.yml
  format: yaml
  label: Smartrr Subscribers API
  slug: smartrr-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartrr/refs/heads/main/openapi/smartrr-openapi.yml
- filename: smartrr-openapi.yml
  format: yaml
  label: Smartrr Orders and Bills API
  slug: smartrr-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartrr/refs/heads/main/openapi/smartrr-openapi.yml
- filename: smartrr-openapi.yml
  format: yaml
  label: Smartrr Plans and Purchasables API
  slug: smartrr-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartrr/refs/heads/main/openapi/smartrr-openapi.yml
- filename: smartrr-openapi.yml
  format: yaml
  label: Smartrr Webhooks API
  slug: smartrr-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartrr/refs/heads/main/openapi/smartrr-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Smartrr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Smartrr secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Smartrr
provider_slug: smartrr
scheme_count: 1
schemes:
- description: Per-organization API access token generated in the Smartrr admin under the Integrations tab (Add Key). Sent on every request in the x-smartrr-access-token header.
  in: header
  name: smartrrAccessToken
  parameter: x-smartrr-access-token
  sources:
  - openapi/smartrr-openapi.yml
  type: apiKey
slug: smartrr-authentication
source_filename: smartrr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/smartrr-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: smartrrAccessToken\n  type: apiKey\n  in: header\n  parameter: x-smartrr-access-token\n  description: Per-organization API access token generated in the Smartrr admin under the Integrations\n    tab (Add Key). Sent on every request in the x-smartrr-access-token header.\n  sources:\n  - openapi/smartrr-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartrr/refs/heads/main/authentication/smartrr-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Subscriptions
- Loyalty
- Shopify
- Ecommerce
- DTC
- Recurring Revenue
- Subscription Management
---
