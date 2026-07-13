---
api_key_in:
- header
- query
api_specs:
- filename: mockaroo-openapi.yml
  format: yaml
  label: Mockaroo API
  slug: mockaroo
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mockaroo/refs/heads/main/openapi/mockaroo-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Mockaroo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mockaroo secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Mockaroo
provider_slug: mockaroo
scheme_count: 2
schemes:
- description: Mockaroo API key passed as a query parameter.
  in: query
  name: apiKeyQuery
  parameter: key
  sources:
  - openapi/mockaroo-openapi.yml
  type: apiKey
- description: Mockaroo API key passed as a request header.
  in: header
  name: apiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/mockaroo-openapi.yml
  type: apiKey
slug: mockaroo-authentication
source_filename: mockaroo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mockaroo-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  description: Mockaroo API key passed as a query parameter.\n  sources:\n  - openapi/mockaroo-openapi.yml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Mockaroo API key passed as a request header.\n  sources:\n  - openapi/mockaroo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mockaroo/refs/heads/main/authentication/mockaroo-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Test Data
- Mock Data
- API Mocking
- Data Generation
- Developer Tools
- QA Testing
- Realistic Data
- Schemas
- Datasets
- Public APIs
---
