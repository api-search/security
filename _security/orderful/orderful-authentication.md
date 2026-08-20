---
api_key_in:
- header
api_specs:
- filename: orderful-conversion-api-openapi.yml
  format: yaml
  label: Orderful Conversion API
  slug: orderful-conversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderful/refs/heads/main/openapi/orderful-conversion-api-openapi.yml
- filename: orderful-delivery-api-openapi.yml
  format: yaml
  label: Orderful Delivery API
  slug: orderful-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderful/refs/heads/main/openapi/orderful-delivery-api-openapi.yml
- filename: orderful-inbox-api-openapi.yml
  format: yaml
  label: Orderful Inbox API
  slug: orderful-inbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderful/refs/heads/main/openapi/orderful-inbox-api-openapi.yml
- filename: orderful-label-api-openapi.yml
  format: yaml
  label: Orderful Label API
  slug: orderful-label-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderful/refs/heads/main/openapi/orderful-label-api-openapi.yml
- filename: orderful-organization-api-openapi.yml
  format: yaml
  label: Orderful Organization API
  slug: orderful-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderful/refs/heads/main/openapi/orderful-organization-api-openapi.yml
- filename: orderful-poller-api-openapi.yml
  format: yaml
  label: Orderful Poller API
  slug: orderful-poller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderful/refs/heads/main/openapi/orderful-poller-api-openapi.yml
- filename: orderful-relationship-api-openapi.yml
  format: yaml
  label: Orderful Relationship API
  slug: orderful-relationship-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderful/refs/heads/main/openapi/orderful-relationship-api-openapi.yml
- filename: orderful-transaction-api-openapi.yml
  format: yaml
  label: Orderful Transaction API
  slug: orderful-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderful/refs/heads/main/openapi/orderful-transaction-api-openapi.yml
- filename: orderful-transaction-v3-api-openapi.yml
  format: yaml
  label: Orderful Transaction (v3) API
  slug: orderful-transaction-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderful/refs/heads/main/openapi/orderful-transaction-v3-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Orderful Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orderful secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Orderful
provider_slug: orderful
scheme_count: 1
schemes:
- in: header
  name: API_KEY
  parameter: orderful-api-key
  sources:
  - openapi/orderful-openapi-original.yml
  type: apiKey
slug: orderful-authentication
source_filename: orderful-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/orderful-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: API_KEY\n  type: apiKey\n  in: header\n  parameter: orderful-api-key\n  sources:\n  - openapi/orderful-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orderful/refs/heads/main/authentication/orderful-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- EDI
- Electronic Data Interchange
- Supply Chain
- B2B
- Logistics
- Retail
- Transaction
- Integration
---
