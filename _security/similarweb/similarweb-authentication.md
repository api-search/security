---
api_key_in:
- header
- query
api_specs:
- filename: llms.txt
  format: yaml
  label: SimilarWeb REST API
  slug: similarweb-rest-api
  spec_type: OpenAPI
  url: https://developers.similarweb.com/llms.txt
- filename: similarweb-batch-api-openapi.yml
  format: yaml
  label: SimilarWeb Batch API
  slug: similarweb-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-batch-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Similarweb Authentication
name_suffix: Authentication
oauth_flows: []
overview: SimilarWeb secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SimilarWeb
provider_slug: similarweb
scheme_count: 2
schemes:
- description: SimilarWeb API key passed as a request header
  in: header
  name: apiKeyHeader
  parameter: api-key
  sources:
  - openapi/similarweb-batch-api-openapi.yml
  - openapi/similarweb-rest-api-openapi.yml
  type: apiKey
- description: SimilarWeb API key passed as a query parameter
  in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/similarweb-rest-api-openapi.yml
  type: apiKey
slug: similarweb-authentication
source_filename: similarweb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/similarweb-batch-api-openapi.yml, openapi/similarweb-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: SimilarWeb API key passed as a request header\n  sources:\n  - openapi/similarweb-batch-api-openapi.yml\n  - openapi/similarweb-rest-api-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: SimilarWeb API key passed as a query parameter\n  sources:\n  - openapi/similarweb-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/authentication/similarweb-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Digital Intelligence
- Web Analytics
- Traffic Analytics
- Competitive Intelligence
- Keyword Analytics
- Audience Demographics
- App Intelligence
- Market Research
- E-commerce
- SEO
---
