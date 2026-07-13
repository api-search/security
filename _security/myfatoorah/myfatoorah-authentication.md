---
api_key_in: []
api_specs:
- filename: myfatoorah-openapi.yml
  format: yaml
  label: MyFatoorah Payments API
  slug: myfatoorah-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myfatoorah/refs/heads/main/openapi/myfatoorah-openapi.yml
- filename: myfatoorah-openapi.yml
  format: yaml
  label: MyFatoorah Invoicing API
  slug: myfatoorah-invoicing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myfatoorah/refs/heads/main/openapi/myfatoorah-openapi.yml
- filename: myfatoorah-openapi.yml
  format: yaml
  label: MyFatoorah Payment Status API
  slug: myfatoorah-payment-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myfatoorah/refs/heads/main/openapi/myfatoorah-openapi.yml
- filename: myfatoorah-openapi.yml
  format: yaml
  label: MyFatoorah Refunds API
  slug: myfatoorah-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myfatoorah/refs/heads/main/openapi/myfatoorah-openapi.yml
- filename: myfatoorah-openapi.yml
  format: yaml
  label: MyFatoorah Embedded Sessions API
  slug: myfatoorah-embedded-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myfatoorah/refs/heads/main/openapi/myfatoorah-openapi.yml
- filename: myfatoorah-openapi.yml
  format: yaml
  label: MyFatoorah Suppliers API
  slug: myfatoorah-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myfatoorah/refs/heads/main/openapi/myfatoorah-openapi.yml
- filename: myfatoorah-openapi.yml
  format: yaml
  label: MyFatoorah Shipping API
  slug: myfatoorah-shipping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myfatoorah/refs/heads/main/openapi/myfatoorah-openapi.yml
- filename: myfatoorah-openapi.yml
  format: yaml
  label: MyFatoorah Recurring Payments API
  slug: myfatoorah-recurring-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myfatoorah/refs/heads/main/openapi/myfatoorah-openapi.yml
- filename: myfatoorah-openapi.yml
  format: yaml
  label: MyFatoorah Webhooks API
  slug: myfatoorah-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myfatoorah/refs/heads/main/openapi/myfatoorah-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Myfatoorah Authentication
name_suffix: Authentication
oauth_flows: []
overview: MyFatoorah secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MyFatoorah
provider_slug: myfatoorah
scheme_count: 1
schemes:
- description: 'MyFatoorah authenticates every REST request with a Bearer API token passed as `Authorization: Bearer {token}`. Tokens are issued from the MyFatoorah portal (log in with the Super Master Account, then Integration Settings -> API Key); up to five tokens can be created per account with custom names, expiration dates, and per-endpoint permissions. Each enabled country requires its own token, and calling an endpoint the token lacks permission for returns HTTP 401 with "The token does not have the required permissions!". A public sandbox demo token is published in the docs for testing against apitest.myfatoorah.com.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/myfatoorah-openapi.yml
  - https://docs.myfatoorah.com/docs/api-key
  - https://docs.myfatoorah.com/docs/authentication
  type: http
slug: myfatoorah-authentication
source_filename: myfatoorah-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/myfatoorah-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    MyFatoorah authenticates every REST request with a Bearer API token passed as\n    `Authorization: Bearer {token}`. Tokens are issued from the MyFatoorah portal\n    (log in with the Super Master Account, then Integration Settings -> API Key);\n    up to five tokens can be created per account with custom names, expiration\n    dates, and per-endpoint permissions. Each enabled country requires its own\n    token, and calling an endpoint the token lacks permission for returns HTTP 401\n    with \"The token does not have the required permissions!\". A public sandbox\n    demo token is published in the docs for testing against apitest.myfatoorah.com.\n  sources:\n  - openapi/myfatoorah-openapi.yml\n  - https://docs.myfatoorah.com/docs/api-key\n  - https://docs.myfatoorah.com/docs/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/myfatoorah/refs/heads/main/authentication/myfatoorah-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Payment Gateway
- Kuwait
- GCC
- MENA
- KNET
- mada
- Benefit
- Invoices
- Cards
- Fintech
---
