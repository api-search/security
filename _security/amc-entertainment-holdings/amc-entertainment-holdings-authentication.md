---
api_key_in:
- header
api_specs:
- filename: amc-entertainment-holdings-barcodes-api-openapi.yml
  format: yaml
  label: AMC Entertainment Holdings Barcodes API
  slug: amc-entertainment-holdings-barcodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amc-entertainment-holdings/refs/heads/main/openapi/amc-entertainment-holdings-barcodes-api-openapi.yml
- filename: amc-entertainment-holdings-concessions-api-openapi.yml
  format: yaml
  label: AMC Entertainment Holdings Concessions API
  slug: amc-entertainment-holdings-concessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amc-entertainment-holdings/refs/heads/main/openapi/amc-entertainment-holdings-concessions-api-openapi.yml
- filename: amc-entertainment-holdings-locations-api-openapi.yml
  format: yaml
  label: AMC Entertainment Holdings Locations API
  slug: amc-entertainment-holdings-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amc-entertainment-holdings/refs/heads/main/openapi/amc-entertainment-holdings-locations-api-openapi.yml
- filename: amc-entertainment-holdings-loyalty-api-openapi.yml
  format: yaml
  label: AMC Entertainment Holdings Loyalty API
  slug: amc-entertainment-holdings-loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amc-entertainment-holdings/refs/heads/main/openapi/amc-entertainment-holdings-loyalty-api-openapi.yml
- filename: amc-entertainment-holdings-markets-api-openapi.yml
  format: yaml
  label: AMC Entertainment Holdings Markets API
  slug: amc-entertainment-holdings-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amc-entertainment-holdings/refs/heads/main/openapi/amc-entertainment-holdings-markets-api-openapi.yml
- filename: amc-entertainment-holdings-media-api-openapi.yml
  format: yaml
  label: AMC Entertainment Holdings Media API
  slug: amc-entertainment-holdings-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amc-entertainment-holdings/refs/heads/main/openapi/amc-entertainment-holdings-media-api-openapi.yml
- filename: amc-entertainment-holdings-movieconfirmations-api-openapi.yml
  format: yaml
  label: AMC Entertainment Holdings MovieConfirmations API
  slug: amc-entertainment-holdings-movieconfirmations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amc-entertainment-holdings/refs/heads/main/openapi/amc-entertainment-holdings-movieconfirmations-api-openapi.yml
- filename: amc-entertainment-holdings-movies-api-openapi.yml
  format: yaml
  label: AMC Entertainment Holdings Movies API
  slug: amc-entertainment-holdings-movies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amc-entertainment-holdings/refs/heads/main/openapi/amc-entertainment-holdings-movies-api-openapi.yml
- filename: amc-entertainment-holdings-orders-api-openapi.yml
  format: yaml
  label: AMC Entertainment Holdings Orders API
  slug: amc-entertainment-holdings-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amc-entertainment-holdings/refs/heads/main/openapi/amc-entertainment-holdings-orders-api-openapi.yml
- filename: amc-entertainment-holdings-refunds-api-openapi.yml
  format: yaml
  label: AMC Entertainment Holdings Refunds API
  slug: amc-entertainment-holdings-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amc-entertainment-holdings/refs/heads/main/openapi/amc-entertainment-holdings-refunds-api-openapi.yml
- filename: amc-entertainment-holdings-seating-api-openapi.yml
  format: yaml
  label: AMC Entertainment Holdings Seating API
  slug: amc-entertainment-holdings-seating-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amc-entertainment-holdings/refs/heads/main/openapi/amc-entertainment-holdings-seating-api-openapi.yml
- filename: amc-entertainment-holdings-showtimes-api-openapi.yml
  format: yaml
  label: AMC Entertainment Holdings Showtimes API
  slug: amc-entertainment-holdings-showtimes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amc-entertainment-holdings/refs/heads/main/openapi/amc-entertainment-holdings-showtimes-api-openapi.yml
- filename: amc-entertainment-holdings-states-api-openapi.yml
  format: yaml
  label: AMC Entertainment Holdings States API
  slug: amc-entertainment-holdings-states-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amc-entertainment-holdings/refs/heads/main/openapi/amc-entertainment-holdings-states-api-openapi.yml
- filename: amc-entertainment-holdings-theatres-api-openapi.yml
  format: yaml
  label: AMC Entertainment Holdings Theatres API
  slug: amc-entertainment-holdings-theatres-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amc-entertainment-holdings/refs/heads/main/openapi/amc-entertainment-holdings-theatres-api-openapi.yml
- filename: amc-entertainment-holdings-wallet-api-openapi.yml
  format: yaml
  label: AMC Entertainment Holdings Wallet API
  slug: amc-entertainment-holdings-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amc-entertainment-holdings/refs/heads/main/openapi/amc-entertainment-holdings-wallet-api-openapi.yml
- filename: amc-entertainment-holdings-webhooks-api-openapi.yml
  format: yaml
  label: AMC Entertainment Holdings Webhooks API
  slug: amc-entertainment-holdings-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amc-entertainment-holdings/refs/heads/main/openapi/amc-entertainment-holdings-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amc Entertainment Holdings Authentication
name_suffix: Authentication
oauth_flows: []
overview: AMC Entertainment Holdings secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AMC Entertainment Holdings
provider_slug: amc-entertainment-holdings
scheme_count: 1
schemes:
- description: AMC vendor API key issued via the AMC Theatres developer portal.
  in: header
  name: VendorKey
  parameter: X-AMC-Vendor-Key
  sources:
  - openapi/amc-theatres-api-openapi.yml
  type: apiKey
slug: amc-entertainment-holdings-authentication
source_filename: amc-entertainment-holdings-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amc-theatres-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: VendorKey\n  type: apiKey\n  in: header\n  parameter: X-AMC-Vendor-Key\n  description: AMC vendor API key issued via the AMC Theatres developer portal.\n  sources:\n  - openapi/amc-theatres-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amc-entertainment-holdings/refs/heads/main/authentication/amc-entertainment-holdings-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Entertainment
- Movies
- Theatres
- Showtimes
- Ticketing
- Concessions
- Loyalty
- Fortune 500
---
