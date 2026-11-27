---
anonymous_access: false
api_key_in: []
api_specs:
- filename: compareanswering-com-enquiry-api-openapi.yml
  format: yaml
  label: Compare Answering Enquiry API
  slug: compareanswering-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compareanswering-com/openapi/compareanswering-com-enquiry-api-openapi.yml
- filename: compareanswering-com-guide-api-openapi.yml
  format: yaml
  label: Compare Answering Guide API
  slug: compareanswering-com-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compareanswering-com/openapi/compareanswering-com-guide-api-openapi.yml
- filename: compareanswering-com-mcp-api-openapi.yml
  format: yaml
  label: Compare Answering MCP API
  slug: compareanswering-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compareanswering-com/openapi/compareanswering-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Compare Answering Authentication
name_suffix: Authentication
oauth_flows: []
overview: Compare Answering secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Compare Answering
provider_slug: compareanswering-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  key_prefix: emk_
  name: accessKey
  required: false
  scheme: bearer
  sources:
  - openapi/compareanswering-com-openapi.yml
  - https://compareanswering.com/openapi.json
  type: http
slug: compareanswering-com-authentication
source_filename: compareanswering-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://compareanswering.com/openapi.json\ndocs: https://compareanswering.com/mcp\nsummary:\n  types:\n  - http\n  optional: true\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  key_prefix: emk_\n  required: false\n  sources:\n  - openapi/compareanswering-com-openapi.yml\n  - https://compareanswering.com/openapi.json\nnotes:\n- 'The provider''s MCP server card (GET https://compareanswering.com/mcp, HTTP 200) declares \"auth\": \"none\" for the Streamable HTTP MCP endpoint; the bearer access key is optional and only raises the free-tier ceiling.'\n- 'No documentation page describing how to obtain an emk_ access key was found; the 429 response text points to \"docs/MCP.md\", which returned HTTP 404 at https://compareanswering.com/docs/MCP.md.'\n"
source_yaml_url: https://artifacts.apis.io/compareanswering-com/authentication/compareanswering-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Answering Services
- Virtual Receptionists
- Price Comparison
- Pricing Data
- Datasets
- MCP
---
