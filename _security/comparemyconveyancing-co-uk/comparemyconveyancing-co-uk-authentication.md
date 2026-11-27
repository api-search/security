---
anonymous_access: false
api_key_in: []
api_specs:
- filename: comparemyconveyancing-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Compare My Conveyancing Enquiry API
  slug: comparemyconveyancing-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comparemyconveyancing-co-uk/openapi/comparemyconveyancing-co-uk-enquiry-api-openapi.yml
- filename: comparemyconveyancing-co-uk-guide-api-openapi.yml
  format: yaml
  label: Compare My Conveyancing Guide API
  slug: comparemyconveyancing-co-uk-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comparemyconveyancing-co-uk/openapi/comparemyconveyancing-co-uk-guide-api-openapi.yml
- filename: comparemyconveyancing-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Compare My Conveyancing MCP API
  slug: comparemyconveyancing-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comparemyconveyancing-co-uk/openapi/comparemyconveyancing-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Compare My Conveyancing Authentication
name_suffix: Authentication
oauth_flows: []
overview: Compare My Conveyancing secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Compare My Conveyancing
provider_slug: comparemyconveyancing-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/comparemyconveyancing-co-uk-openapi.yml
  type: http
slug: comparemyconveyancing-co-uk-authentication
source_filename: comparemyconveyancing-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://comparemyconveyancing.co.uk/openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires\n    one.'\n  sources:\n  - openapi/comparemyconveyancing-co-uk-openapi.yml\ndocs: https://comparemyconveyancing.co.uk/mcp\noptional: true\nnote: 'The bearer key is optional: the OpenAPI sets no top-level security requirement, and the MCP server card at\n  https://comparemyconveyancing.co.uk/mcp (GET, 200, 2026-11-04) declares \"auth\":\"none\". The spec says an emk_ key\n  gives a named budget and is required for the bulk entity export. No page documenting how to obtain a key was found\n  (docs/MCP.md referenced in the 429 response returns 404).'\n"
source_yaml_url: https://artifacts.apis.io/comparemyconveyancing-co-uk/authentication/comparemyconveyancing-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Conveyancing
- Property
- Real Estate
- Legal
- United Kingdom
- Calculators
- Open Data
- MCP
---
