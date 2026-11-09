---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bagsthatpay-com-dataset-api-openapi.yml
  format: yaml
  label: Bags That Pay Dataset API
  slug: bagsthatpay-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bagsthatpay-com/openapi/bagsthatpay-com-dataset-api-openapi.yml
- filename: bagsthatpay-com-enquiry-api-openapi.yml
  format: yaml
  label: Bags That Pay Enquiry API
  slug: bagsthatpay-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bagsthatpay-com/openapi/bagsthatpay-com-enquiry-api-openapi.yml
- filename: bagsthatpay-com-entities-api-openapi.yml
  format: yaml
  label: Bags That Pay Entities API
  slug: bagsthatpay-com-entities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bagsthatpay-com/openapi/bagsthatpay-com-entities-api-openapi.yml
- filename: bagsthatpay-com-listing-api-openapi.yml
  format: yaml
  label: Bags That Pay Listing API
  slug: bagsthatpay-com-listing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bagsthatpay-com/openapi/bagsthatpay-com-listing-api-openapi.yml
- filename: bagsthatpay-com-mcp-api-openapi.yml
  format: yaml
  label: Bags That Pay MCP API
  slug: bagsthatpay-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bagsthatpay-com/openapi/bagsthatpay-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Bagsthatpay Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bags That Pay secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bags That Pay
provider_slug: bagsthatpay-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/bagsthatpay-com-openapi.json
  type: http
slug: bagsthatpay-com-authentication
source_filename: bagsthatpay-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/bagsthatpay-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/bagsthatpay-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/bagsthatpay-com/authentication/bagsthatpay-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Finance
- Tokenization
- Treasury-Bills
- DeFi
- Data Aggregation
---
