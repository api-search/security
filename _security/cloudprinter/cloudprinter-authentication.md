---
api_key_in:
- header
api_specs:
- filename: cloudprinter-openapi.yml
  format: yaml
  label: Cloudprinter Orders API
  slug: cloudprinter-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudprinter/refs/heads/main/openapi/cloudprinter-openapi.yml
- filename: cloudprinter-openapi.yml
  format: yaml
  label: Cloudprinter Products & Pricing API
  slug: cloudprinter-products-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudprinter/refs/heads/main/openapi/cloudprinter-openapi.yml
- filename: cloudprinter-openapi.yml
  format: yaml
  label: Cloudprinter Quotes API
  slug: cloudprinter-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudprinter/refs/heads/main/openapi/cloudprinter-openapi.yml
- filename: cloudprinter-openapi.yml
  format: yaml
  label: Cloudprinter Signal Webhooks API
  slug: cloudprinter-signal-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudprinter/refs/heads/main/openapi/cloudprinter-openapi.yml
- filename: cloudprinter-openapi.yml
  format: yaml
  label: Cloudprinter Files API
  slug: cloudprinter-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudprinter/refs/heads/main/openapi/cloudprinter-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cloudprinter Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cloudprinter secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cloudprinter
provider_slug: cloudprinter
scheme_count: 1
schemes:
- description: CloudCore API key from the Cloudprinter.com dashboard. The API key is supplied in the JSON request body as the "apikey" field on every call; this scheme is declared as a header for tooling compatibility.
  in: header
  name: apikeyBody
  parameter: apikey
  sources:
  - openapi/cloudprinter-openapi.yml
  type: apiKey
slug: cloudprinter-authentication
source_filename: cloudprinter-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloudprinter-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apikeyBody\n  type: apiKey\n  in: header\n  parameter: apikey\n  description: CloudCore API key from the Cloudprinter.com dashboard. The API key is supplied\n    in the JSON request body as the \"apikey\" field on every call; this scheme is declared as\n    a header for tooling compatibility.\n  sources:\n  - openapi/cloudprinter-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudprinter/refs/heads/main/authentication/cloudprinter-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Print on Demand
- Print Fulfillment
- Printing
- Orders
- Logistics
---
