---
api_key_in: []
api_specs:
- filename: wompi-openapi.yml
  format: yaml
  label: Wompi Transactions API
  slug: wompi-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wompi/refs/heads/main/openapi/wompi-openapi.yml
- filename: wompi-openapi.yml
  format: yaml
  label: Wompi Tokenization API
  slug: wompi-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wompi/refs/heads/main/openapi/wompi-openapi.yml
- filename: wompi-openapi.yml
  format: yaml
  label: Wompi Payment Sources API
  slug: wompi-payment-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wompi/refs/heads/main/openapi/wompi-openapi.yml
- filename: wompi-openapi.yml
  format: yaml
  label: Wompi PSE API
  slug: wompi-pse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wompi/refs/heads/main/openapi/wompi-openapi.yml
- filename: wompi-openapi.yml
  format: yaml
  label: Wompi Payment Links API
  slug: wompi-payment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wompi/refs/heads/main/openapi/wompi-openapi.yml
- filename: wompi-openapi.yml
  format: yaml
  label: Wompi Merchants & Acceptance Tokens API
  slug: wompi-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wompi/refs/heads/main/openapi/wompi-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Wompi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wompi secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Wompi
provider_slug: wompi
scheme_count: 2
schemes:
- bearerFormat: apiKey
  keyPrefix: pub_prod_ / pub_test_
  name: public_key
  scheme: bearer
  sources:
  - openapi/wompi-openapi.yml
  type: http
  usage: Client-side safe; tokenization, merchant read, transaction create/read, PSE catalog.
- bearerFormat: apiKey
  keyPrefix: prv_prod_ / prv_test_
  name: private_key
  scheme: bearer
  sources:
  - openapi/wompi-openapi.yml
  type: http
  usage: Server-side only; payment sources, voids, payment links.
slug: wompi-authentication
source_filename: wompi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/wompi-openapi.yml\nsummary:\n  types:\n  - http\nnotes: >-\n  Wompi uses two HTTP Bearer keys per environment. The PUBLIC key (pub_prod_ /\n  pub_test_) is browser-safe and authorizes merchant reads, card/Nequi\n  tokenization, PSE catalog, and transaction create/read. The PRIVATE key\n  (prv_prod_ / prv_test_) is server-side only and authorizes payment sources,\n  voids, and payment links. Creating transactions additionally requires a\n  presigned acceptance token and an integrity signature (firma de integridad)\n  computed from an events/integrity secret; webhook events are validated with an\n  asymmetric checksum in the X-Event-Checksum header.\nschemes:\n- name: public_key\n  type: http\n  scheme: bearer\n  bearerFormat: apiKey\n  keyPrefix: pub_prod_ / pub_test_\n  usage: Client-side safe; tokenization, merchant read, transaction create/read, PSE catalog.\n  sources:\n  - openapi/wompi-openapi.yml\n- name: private_key\n\
  \  type: http\n  scheme: bearer\n  bearerFormat: apiKey\n  keyPrefix: prv_prod_ / prv_test_\n  usage: Server-side only; payment sources, voids, payment links.\n  sources:\n  - openapi/wompi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wompi/refs/heads/main/authentication/wompi-authentication.yml
summary_line: http · 2 schemes
tags:
- Payments
- Fintech
- Colombia
- LatAm
- Payment Gateway
- PSE
- Nequi
---
