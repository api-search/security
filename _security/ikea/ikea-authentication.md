---
api_key_in:
- header
api_specs:
- filename: ikea-product-catalog-openapi.yml
  format: yaml
  label: IKEA Product Catalog API (Unofficial)
  slug: product-catalog
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ikea/main/openapi/ikea-product-catalog-openapi.yml
- filename: ikea-search-openapi.yml
  format: yaml
  label: IKEA Search API (Unofficial)
  slug: search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ikea/main/openapi/ikea-search-openapi.yml
- filename: ikea-sales-item-openapi.yml
  format: yaml
  label: IKEA Sales Item API (Unofficial)
  slug: sales-item
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ikea/main/openapi/ikea-sales-item-openapi.yml
- filename: ikea-after-purchase-ordering-openapi.yml
  format: yaml
  label: IKEA After Purchase Ordering API (Unofficial)
  slug: after-purchase-ordering
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ikea/main/openapi/ikea-after-purchase-ordering-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ikea Authentication
name_suffix: Authentication
oauth_flows: []
overview: IKEA secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: IKEA
provider_slug: ikea
scheme_count: 1
schemes:
- description: 'Client specific identifier (Akamai API Gateway) required for API access


    ## Available Client IDs


    The following public client IDs are available:


    - `ef382663-a2a5-40d4-8afe-f0634821c0ed`

    - `b6c117e5-ae61-4ef5-b4cc-e0b1e37f0631`

    - `da465052-7912-43b2-82fa-9dc39cdccef8`



    ## How to Find Client IDs


    Visit any IKEA product page (e.g., [BILLY Bookcase](https://www.ikea.com/gb/en/p/billy-bookcase-white-'
  in: header
  name: X-Client-ID
  parameter: X-Client-ID
  sources:
  - openapi/ikea-sales-item-openapi.yml
  type: apiKey
slug: ikea-authentication
source_filename: ikea-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ikea-sales-item-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: X-Client-ID\n  type: apiKey\n  in: header\n  parameter: X-Client-ID\n  description: |-\n    Client specific identifier (Akamai API Gateway) required for API access\n\n    ## Available Client IDs\n\n    The following public client IDs are available:\n\n    - `ef382663-a2a5-40d4-8afe-f0634821c0ed`\n    - `b6c117e5-ae61-4ef5-b4cc-e0b1e37f0631`\n    - `da465052-7912-43b2-82fa-9dc39cdccef8`\n\n\n    ## How to Find Client IDs\n\n    Visit any IKEA product page (e.g., [BILLY Bookcase](https://www.ikea.com/gb/en/p/billy-bookcase-white-\n  sources:\n  - openapi/ikea-sales-item-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ikea/refs/heads/main/authentication/ikea-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Retail
- Home Furnishings
- Consumer Products
- Opensource
- Community
- Unofficial API
- Smart Home
---
