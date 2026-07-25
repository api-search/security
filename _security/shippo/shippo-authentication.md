---
api_key_in: []
api_specs:
- filename: shippo-addresses-api-openapi.yml
  format: yaml
  label: Shippo Addresses API
  slug: shippo-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippo/refs/heads/main/openapi/shippo-addresses-api-openapi.yml
- filename: shippo-carrier-accounts-api-openapi.yml
  format: yaml
  label: Shippo Carrier Accounts API
  slug: shippo-carrier-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippo/refs/heads/main/openapi/shippo-carrier-accounts-api-openapi.yml
- filename: shippo-parcels-api-openapi.yml
  format: yaml
  label: Shippo Parcels API
  slug: shippo-parcels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippo/refs/heads/main/openapi/shippo-parcels-api-openapi.yml
- filename: shippo-rates-api-openapi.yml
  format: yaml
  label: Shippo Rates API
  slug: shippo-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippo/refs/heads/main/openapi/shippo-rates-api-openapi.yml
- filename: shippo-refunds-api-openapi.yml
  format: yaml
  label: Shippo Refunds API
  slug: shippo-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippo/refs/heads/main/openapi/shippo-refunds-api-openapi.yml
- filename: shippo-shipments-api-openapi.yml
  format: yaml
  label: Shippo Shipments API
  slug: shippo-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippo/refs/heads/main/openapi/shippo-shipments-api-openapi.yml
- filename: shippo-tracking-api-openapi.yml
  format: yaml
  label: Shippo Tracking API
  slug: shippo-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippo/refs/heads/main/openapi/shippo-tracking-api-openapi.yml
- filename: shippo-transactions-api-openapi.yml
  format: yaml
  label: Shippo Transactions API
  slug: shippo-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippo/refs/heads/main/openapi/shippo-transactions-api-openapi.yml
- filename: shippo-webhooks-api-openapi.yml
  format: yaml
  label: Shippo Webhooks API
  slug: shippo-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippo/refs/heads/main/openapi/shippo-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Shippo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shippo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Shippo
provider_slug: shippo
scheme_count: 1
schemes:
- description: Shippo API token (prefix with "ShippoToken ")
  name: ShippoToken
  scheme: bearer
  sources:
  - openapi/shippo-openapi.yml
  type: http
slug: shippo-authentication
source_filename: shippo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shippo-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: ShippoToken\n  type: http\n  scheme: bearer\n  description: Shippo API token (prefix with \"ShippoToken \")\n  sources:\n  - openapi/shippo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shippo/refs/heads/main/authentication/shippo-authentication.yml
summary_line: http · 1 scheme
tags:
- Ecommerce
- Labels
- Logistics
- Returns
- Shipping
- Tracking
---
