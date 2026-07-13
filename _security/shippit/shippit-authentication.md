---
api_key_in: []
api_specs:
- filename: shippit-openapi.yml
  format: yaml
  label: Shippit Quote API
  slug: shippit-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippit/refs/heads/main/openapi/shippit-openapi.yml
- filename: shippit-openapi.yml
  format: yaml
  label: Shippit Orders API
  slug: shippit-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippit/refs/heads/main/openapi/shippit-openapi.yml
- filename: shippit-openapi.yml
  format: yaml
  label: Shippit Book API
  slug: shippit-book-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippit/refs/heads/main/openapi/shippit-openapi.yml
- filename: shippit-openapi.yml
  format: yaml
  label: Shippit Label API
  slug: shippit-label-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippit/refs/heads/main/openapi/shippit-openapi.yml
- filename: shippit-openapi.yml
  format: yaml
  label: Shippit Tracking API
  slug: shippit-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippit/refs/heads/main/openapi/shippit-openapi.yml
- filename: shippit-openapi.yml
  format: yaml
  label: Shippit Merchant API
  slug: shippit-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippit/refs/heads/main/openapi/shippit-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Shippit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shippit secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Shippit
provider_slug: shippit
scheme_count: 1
schemes:
- description: 'Per-merchant API key (referred to in Shippit docs as the API Secret) passed as an HTTP Bearer token: `Authorization: Bearer YOUR_API_KEY`. The key is obtained from the Shippit merchant dashboard. Shippit also recommends sending `user-agent` and `x-shippit-platform` headers to identify the integration. Use a staging key against the staging base URL (https://app.staging.shippit.com/api/3) and a production key against production (https://app.shippit.com/api/3). No HMAC request signing is documented.'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://developer.shippit.com/dev_guide/using_apis/authentication.html
  - https://developer.shippit.com/dev_guide/using_apis/using_apis.html
  type: http
slug: shippit-authentication
source_filename: shippit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: https://developer.shippit.com/dev_guide/using_apis/authentication.html\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Per-merchant API key (referred to in Shippit docs as the API Secret)\n    passed as an HTTP Bearer token: `Authorization: Bearer YOUR_API_KEY`. The key\n    is obtained from the Shippit merchant dashboard. Shippit also recommends sending\n    `user-agent` and `x-shippit-platform` headers to identify the integration. Use\n    a staging key against the staging base URL (https://app.staging.shippit.com/api/3)\n    and a production key against production (https://app.shippit.com/api/3). No HMAC\n    request signing is documented.'\n  sources:\n  - https://developer.shippit.com/dev_guide/using_apis/authentication.html\n  - https://developer.shippit.com/dev_guide/using_apis/using_apis.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shippit/refs/heads/main/authentication/shippit-authentication.yml
summary_line: http · 1 scheme
tags:
- Shipping
- Logistics
- Fulfillment
- Australia
- APAC
- Multi-Carrier
- Labels
- Tracking
- Parcels
- E-commerce Logistics
- SaaS
---
