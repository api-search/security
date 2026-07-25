---
api_key_in: []
api_specs:
- filename: seel-bill-api-openapi.yml
  format: yaml
  label: Seel Bill API
  slug: seel-bill-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seel/refs/heads/main/openapi/seel-bill-api-openapi.yml
- filename: seel-claim-api-openapi.yml
  format: yaml
  label: Seel Claim API
  slug: seel-claim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seel/refs/heads/main/openapi/seel-claim-api-openapi.yml
- filename: seel-contract-api-openapi.yml
  format: yaml
  label: Seel Contract API
  slug: seel-contract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seel/refs/heads/main/openapi/seel-contract-api-openapi.yml
- filename: seel-event-api-openapi.yml
  format: yaml
  label: Seel Event API
  slug: seel-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seel/refs/heads/main/openapi/seel-event-api-openapi.yml
- filename: seel-fulfillment-api-openapi.yml
  format: yaml
  label: Seel Fulfillment API
  slug: seel-fulfillment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seel/refs/heads/main/openapi/seel-fulfillment-api-openapi.yml
- filename: seel-merchant-api-openapi.yml
  format: yaml
  label: Seel Merchant API
  slug: seel-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seel/refs/heads/main/openapi/seel-merchant-api-openapi.yml
- filename: seel-order-api-openapi.yml
  format: yaml
  label: Seel Order API
  slug: seel-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seel/refs/heads/main/openapi/seel-order-api-openapi.yml
- filename: seel-product-api-openapi.yml
  format: yaml
  label: Seel Product API
  slug: seel-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seel/refs/heads/main/openapi/seel-product-api-openapi.yml
- filename: seel-quote-api-openapi.yml
  format: yaml
  label: Seel Quote API
  slug: seel-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seel/refs/heads/main/openapi/seel-quote-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Seel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Seel declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Seel
provider_slug: seel
scheme_count: 1
schemes:
- description: Per-merchant secret API key issued by Seel (request via merchant@seel.com). Sent on every request; must never be exposed in client-side code or public repositories.
  id: SeelApiKey
  in: header
  name: X-Seel-Api-Key
  required: true
  type: apiKey
slug: seel-authentication
source_filename: seel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  https://developer.seel.com/reference/introduction.md and per-operation\n  reference pages. Seel authenticates every request with a per-merchant API key\n  in the X-Seel-Api-Key header, paired with an X-Seel-Api-Version header to\n  select the API version. No OAuth2/OIDC surface is documented.\nbase_url: https://api-test.seel.com/v1\nschemes:\n  - id: SeelApiKey\n    type: apiKey\n    in: header\n    name: X-Seel-Api-Key\n    description: >-\n      Per-merchant secret API key issued by Seel (request via merchant@seel.com).\n      Sent on every request; must never be exposed in client-side code or public\n      repositories.\n    required: true\nversion_header:\n  name: X-Seel-Api-Version\n  example: 2.6.0\n  description: Selects the API version (e.g. 2.1.0, 2.3.0, 2.6.0).\ntransport:\n  https_required: true\n  notes: All requests must use HTTPS; plain HTTP calls fail.\noauth2: false\nopenid_connect: false\nmutual_tls:\
  \ false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seel/refs/heads/main/authentication/seel-authentication.yml
summary_line: 1 scheme
tags:
- Company
- E-commerce
- Insurance
- Post-Purchase
- Returns
- Extended Warranty
- Fraud
- Payments
---
