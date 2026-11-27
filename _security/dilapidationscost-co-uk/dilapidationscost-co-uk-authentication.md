---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dilapidationscost-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Dilapidations Cost Enquiry API
  slug: dilapidationscost-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dilapidationscost-co-uk/openapi/dilapidationscost-co-uk-enquiry-api-openapi.yml
- filename: dilapidationscost-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Dilapidations Cost MCP API
  slug: dilapidationscost-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dilapidationscost-co-uk/openapi/dilapidationscost-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Dilapidations Cost Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dilapidations Cost secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dilapidations Cost
provider_slug: dilapidationscost-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  key_prefix: emk_
  name: accessKey
  required: false
  scheme: bearer
  sources:
  - openapi/dilapidationscost-co-uk-openapi.yml
  type: http
slug: dilapidationscost-co-uk-authentication
source_filename: dilapidationscost-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://dilapidationscost.co.uk/openapi.json\ndocs: https://dilapidationscost.co.uk/mcp\nsummary:\n  types:\n  - http\n  optional: true\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires\n    one.'\n  key_prefix: emk_\n  required: false\n  sources:\n  - openapi/dilapidationscost-co-uk-openapi.yml\nnote: 'Every tool operation declares security [{}, {accessKey: []}], i.e. anonymous OR bearer access key. The MCP\n  card at GET https://dilapidationscost.co.uk/mcp (HTTP 200, probed 2026-11-05) states \"auth\":\"none\" for the streamable-http\n  MCP endpoint. No documented way to obtain an emk_ key was found; no OAuth.'\n"
source_yaml_url: https://artifacts.apis.io/dilapidationscost-co-uk/authentication/dilapidationscost-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Dilapidations
- Commercial Property
- Surveying
- Real Estate
- Leases
- United Kingdom
- Datasets
---
