---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cryptoexchangecomparehq-com-dataset-api-openapi.yml
  format: yaml
  label: Crypto Exchange Compare HQ Dataset API
  slug: cryptoexchangecomparehq-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cryptoexchangecomparehq-com/openapi/cryptoexchangecomparehq-com-dataset-api-openapi.yml
- filename: cryptoexchangecomparehq-com-enquiry-api-openapi.yml
  format: yaml
  label: Crypto Exchange Compare HQ Enquiry API
  slug: cryptoexchangecomparehq-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cryptoexchangecomparehq-com/openapi/cryptoexchangecomparehq-com-enquiry-api-openapi.yml
- filename: cryptoexchangecomparehq-com-mcp-api-openapi.yml
  format: yaml
  label: Crypto Exchange Compare HQ MCP API
  slug: cryptoexchangecomparehq-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cryptoexchangecomparehq-com/openapi/cryptoexchangecomparehq-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Crypto Exchange Compare HQ Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crypto Exchange Compare HQ secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Crypto Exchange Compare HQ
provider_slug: cryptoexchangecomparehq-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/cryptoexchangecomparehq-com-openapi.json
  type: http
slug: cryptoexchangecomparehq-com-authentication
source_filename: cryptoexchangecomparehq-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/cryptoexchangecomparehq-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/cryptoexchangecomparehq-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/cryptoexchangecomparehq-com/authentication/cryptoexchangecomparehq-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Cryptocurrency
- Exchange
- Fees
- Comparison
- Data
---
