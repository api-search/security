---
api_key_in:
- header
api_specs:
- filename: aqueduct-accountowner-api-openapi.yml
  format: yaml
  label: Aqueduct AccountOwner API
  slug: aqueduct-accountowner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aqueduct/refs/heads/main/openapi/aqueduct-accountowner-api-openapi.yml
- filename: aqueduct-bill-api-openapi.yml
  format: yaml
  label: Aqueduct Bill API
  slug: aqueduct-bill-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aqueduct/refs/heads/main/openapi/aqueduct-bill-api-openapi.yml
- filename: aqueduct-invoice-api-openapi.yml
  format: yaml
  label: Aqueduct Invoice API
  slug: aqueduct-invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aqueduct/refs/heads/main/openapi/aqueduct-invoice-api-openapi.yml
- filename: aqueduct-invoicelineitem-api-openapi.yml
  format: yaml
  label: Aqueduct InvoiceLineItem API
  slug: aqueduct-invoicelineitem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aqueduct/refs/heads/main/openapi/aqueduct-invoicelineitem-api-openapi.yml
- filename: aqueduct-pricemodel-api-openapi.yml
  format: yaml
  label: Aqueduct PriceModel API
  slug: aqueduct-pricemodel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aqueduct/refs/heads/main/openapi/aqueduct-pricemodel-api-openapi.yml
- filename: aqueduct-productpurchases-api-openapi.yml
  format: yaml
  label: Aqueduct ProductPurchases API
  slug: aqueduct-productpurchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aqueduct/refs/heads/main/openapi/aqueduct-productpurchases-api-openapi.yml
- filename: aqueduct-products-api-openapi.yml
  format: yaml
  label: Aqueduct Products API
  slug: aqueduct-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aqueduct/refs/heads/main/openapi/aqueduct-products-api-openapi.yml
- filename: aqueduct-provisioning-api-openapi.yml
  format: yaml
  label: Aqueduct Provisioning API
  slug: aqueduct-provisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aqueduct/refs/heads/main/openapi/aqueduct-provisioning-api-openapi.yml
- filename: aqueduct-subscriptions-api-openapi.yml
  format: yaml
  label: Aqueduct Subscriptions API
  slug: aqueduct-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aqueduct/refs/heads/main/openapi/aqueduct-subscriptions-api-openapi.yml
- filename: aqueduct-webhooks-api-openapi.yml
  format: yaml
  label: Aqueduct Webhooks API
  slug: aqueduct-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aqueduct/refs/heads/main/openapi/aqueduct-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Aqueduct Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aqueduct secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Aqueduct
provider_slug: aqueduct
scheme_count: 1
schemes:
- format: Api-Key {key}
  in: header
  name: bearerAuth
  parameter: Authorization
  sources:
  - openapi/aqueduct-openapi.json
  type: apiKey
slug: aqueduct-authentication
source_filename: aqueduct-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/aqueduct-openapi.json\ndocs: https://docs.tryaqueduct.com/reference/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nnotes: >-\n  Aqueduct authenticates every request with an API key issued from the dashboard\n  (dashboard.tryaqueduct.com settings page). The key is sent in the Authorization\n  header using the literal prefix \"Api-Key\", i.e. `Authorization: Api-Key {key}`.\n  All requests must be made over HTTPS. There is no OAuth surface. The OpenAPI\n  models this as an apiKey scheme (named \"bearerAuth\" in the spec) in the\n  Authorization header.\nschemes:\n- name: bearerAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Api-Key {key}'\n  sources:\n  - openapi/aqueduct-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aqueduct/refs/heads/main/authentication/aqueduct-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Fintech
- Billing
- Invoicing
- Metering
- Usage-Based
- Subscription
- Payments
---
