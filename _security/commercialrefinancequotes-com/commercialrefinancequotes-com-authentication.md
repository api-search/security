---
anonymous_access: false
api_key_in: []
api_specs:
- filename: commercialrefinancequotes-com-dataset-api-openapi.yml
  format: yaml
  label: Commercial Refinance Quotes Dataset API
  slug: commercialrefinancequotes-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commercialrefinancequotes-com/openapi/commercialrefinancequotes-com-dataset-api-openapi.yml
- filename: commercialrefinancequotes-com-enquiry-api-openapi.yml
  format: yaml
  label: Commercial Refinance Quotes Enquiry API
  slug: commercialrefinancequotes-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commercialrefinancequotes-com/openapi/commercialrefinancequotes-com-enquiry-api-openapi.yml
- filename: commercialrefinancequotes-com-mcp-api-openapi.yml
  format: yaml
  label: Commercial Refinance Quotes MCP API
  slug: commercialrefinancequotes-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commercialrefinancequotes-com/openapi/commercialrefinancequotes-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Commercial Refinance Quotes Authentication
name_suffix: Authentication
oauth_flows: []
overview: Commercial Refinance Quotes secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Commercial Refinance Quotes
provider_slug: commercialrefinancequotes-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  key_prefix: emk_
  name: accessKey
  optional: true
  scheme: bearer
  sources:
  - openapi/commercialrefinancequotes-com-openapi.yml
  type: http
slug: commercialrefinancequotes-com-authentication
source_filename: commercialrefinancequotes-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://commercialrefinancequotes.com/mcp\ndocs: https://commercialrefinancequotes.com/mcp\nsummary:\n  types:\n  - http\n  anonymous_access: true\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  optional: true\n  key_prefix: emk_\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/commercialrefinancequotes-com-openapi.yml\nnote: >-\n  The OpenAPI declares the optional bearer accessKey scheme but applies no global or per-operation\n  security requirement. The MCP card (GET https://commercialrefinancequotes.com/mcp, HTTP 200) states\n  \"auth\": \"none\" for the streamable-http MCP endpoint. No page was found documenting how to obtain an\n  emk_ key (https://commercialrefinancequotes.com/docs/MCP.md, referenced by the 429 response, returned 404).\n"
source_yaml_url: https://artifacts.apis.io/commercialrefinancequotes-com/authentication/commercialrefinancequotes-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Commercial Real Estate
- Refinance
- Lending
- Mortgage
- Financial Data
- Datasets
---
