---
api_key_in:
- header
api_specs:
- filename: komerce-shipping-cost-openapi.yml
  format: yaml
  label: RajaOngkir Shipping Cost API
  slug: shipping-cost
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/komerce/refs/heads/main/openapi/komerce-shipping-cost-openapi.yml
- filename: komerce-shipping-delivery-openapi.yml
  format: yaml
  label: Komerce Shipping Delivery API (Komship)
  slug: shipping-delivery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/komerce/refs/heads/main/openapi/komerce-shipping-delivery-openapi.yml
- filename: komerce-payment-openapi.yml
  format: yaml
  label: Komerce Payment Service API
  slug: payment
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/komerce/refs/heads/main/openapi/komerce-payment-openapi.yml
- filename: komerce-qrisly-openapi.yml
  format: yaml
  label: Komerce QRISLY API
  slug: qrisly
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/komerce/refs/heads/main/openapi/komerce-qrisly-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Komerce Authentication
name_suffix: Authentication
oauth_flows: []
overview: Komerce secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Komerce
provider_slug: komerce
scheme_count: 3
schemes:
- description: Payment API key from the Collaborator dashboard — the same key used for Komerce Shipping (RajaOngkir). Sandbox keys use the sandbox prefix, production keys the live prefix.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/komerce-payment-openapi.yml
  - openapi/komerce-shipping-delivery-openapi.yml
  type: apiKey
- description: QRISLY API key generated from the RajaOngkir Collaborator dashboard (Developer -> API Settings -> Generate New API Key).
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/komerce-qrisly-openapi.yml
  type: apiKey
- description: Shipping Cost API key from the Collaborator dashboard (Developer -> Settings -> Api Key).
  in: header
  name: ApiKeyAuth
  parameter: key
  sources:
  - openapi/komerce-shipping-cost-openapi.yml
  type: apiKey
slug: komerce-authentication
source_filename: komerce-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/komerce-payment-openapi.yml, openapi/komerce-qrisly-openapi.yml, openapi/komerce-shipping-cost-openapi.yml,\n  openapi/komerce-shipping-delivery-openapi.yml\ndocs:\n- https://rajaongkir.com/docs/shipping-cost/getting_started/apikey\n- https://rajaongkir.com/docs/delivery-order-api/getting_started/api-key\n- https://rajaongkir.com/docs/payment-api/getting-started/authentication\n- https://rajaongkir.com/docs/qrisly/getting-started/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  note: >-\n    Every Komerce surface uses a header API key and nothing else — no OAuth 2.0, OIDC, basic,\n    bearer or mTLS. Crucially the keys are per-product and NOT interchangeable: the docs warn\n    explicitly against using a key issued for one service against another. Keys are issued and\n    rotated from the Collaborator dashboard under Developer -> Settings -> Api Key. Sandbox and\n    production\
  \ require separate keys, and a sandbox key will not work in production without\n    administrator approval. HTTPS is required.\n  issuance: https://collaborator.komerce.id/registration\n  dashboard: https://collaborator.komerce.id\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Payment API key from the Collaborator dashboard — the same key used for Komerce\n    Shipping (RajaOngkir). Sandbox keys use the sandbox prefix, production keys the live prefix.\n  sources:\n  - openapi/komerce-payment-openapi.yml\n  - openapi/komerce-shipping-delivery-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: QRISLY API key generated from the RajaOngkir Collaborator dashboard (Developer\n    -> API Settings -> Generate New API Key).\n  sources:\n  - openapi/komerce-qrisly-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: key\n  description: Shipping Cost API key from the Collaborator\
  \ dashboard (Developer -> Settings\n    -> Api Key).\n  sources:\n  - openapi/komerce-shipping-cost-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/komerce/refs/heads/main/authentication/komerce-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Shipping
- Logistics
- E-Commerce
- Payments
- QRIS
- Indonesia
- Couriers
- Tracking
- Fulfillment
---
