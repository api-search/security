---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: arcandledger-com-deadlines-api-openapi.yml
  format: yaml
  label: arcandledger-com Deadlines API
  slug: arcandledger-com-deadlines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcandledger-com/openapi/arcandledger-com-deadlines-api-openapi.yml
- filename: arcandledger-com-interest-rates-api-openapi.yml
  format: yaml
  label: arcandledger-com Interest Rates API
  slug: arcandledger-com-interest-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcandledger-com/openapi/arcandledger-com-interest-rates-api-openapi.yml
- filename: arcandledger-com-notices-api-openapi.yml
  format: yaml
  label: arcandledger-com Notices API
  slug: arcandledger-com-notices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcandledger-com/openapi/arcandledger-com-notices-api-openapi.yml
- filename: arcandledger-com-openapi-json-api-openapi.yml
  format: yaml
  label: arcandledger-com Openapi.json API
  slug: arcandledger-com-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcandledger-com/openapi/arcandledger-com-openapi-json-api-openapi.yml
- filename: arcandledger-com-tax-documents-api-openapi.yml
  format: yaml
  label: arcandledger-com Tax Documents API
  slug: arcandledger-com-tax-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcandledger-com/openapi/arcandledger-com-tax-documents-api-openapi.yml
- filename: arcandledger-com-tax-parameters-api-openapi.yml
  format: yaml
  label: arcandledger-com Tax Parameters API
  slug: arcandledger-com-tax-parameters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcandledger-com/openapi/arcandledger-com-tax-parameters-api-openapi.yml
- filename: arcandledger-com-vintages-api-openapi.yml
  format: yaml
  label: arcandledger-com Vintages API
  slug: arcandledger-com-vintages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcandledger-com/openapi/arcandledger-com-vintages-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Arcandledger Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: arcandledger-com secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: arcandledger-com
provider_slug: arcandledger-com
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: X-Api-Key
  sources:
  - openapi/arcandledger-com-openapi.json
  type: apiKey
slug: arcandledger-com-authentication
source_filename: arcandledger-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/arcandledger-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/arcandledger-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/arcandledger-com/authentication/arcandledger-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Accounting
- Tax
- Bookkeeping
- Financial Services
- Los Angeles
---
