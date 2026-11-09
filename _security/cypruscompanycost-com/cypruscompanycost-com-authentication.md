---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cypruscompanycost-com-enquiry-api-openapi.yml
  format: yaml
  label: Cyprus Company Cost Enquiry API
  slug: cypruscompanycost-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cypruscompanycost-com/openapi/cypruscompanycost-com-enquiry-api-openapi.yml
- filename: cypruscompanycost-com-mcp-api-openapi.yml
  format: yaml
  label: Cyprus Company Cost MCP API
  slug: cypruscompanycost-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cypruscompanycost-com/openapi/cypruscompanycost-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cypruscompanycost Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cyprus Company Cost secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cyprus Company Cost
provider_slug: cypruscompanycost-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  key_prefix: emk_
  name: accessKey
  required: false
  scheme: bearer
  sources:
  - openapi/cypruscompanycost-com-openapi.yml
  - https://cypruscompanycost.com/openapi.json
  type: http
slug: cypruscompanycost-com-authentication
source_filename: cypruscompanycost-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://cypruscompanycost.com/mcp\ndocs: https://cypruscompanycost.com/mcp\nsummary:\n  types:\n  - http\n  anonymous_access: true\n  note: 'The MCP server card (GET https://cypruscompanycost.com/mcp, HTTP 200) states \"auth\": \"none\". The OpenAPI declares\n    an optional bearer access key (emk_...) that raises the free-tier ceiling; no docs page describes how a key is obtained.'\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  required: false\n  key_prefix: emk_\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'\n  sources:\n  - openapi/cypruscompanycost-com-openapi.yml\n  - https://cypruscompanycost.com/openapi.json\n"
source_yaml_url: https://artifacts.apis.io/cypruscompanycost-com/authentication/cypruscompanycost-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Cyprus
- Company Formation
- Corporate Tax
- Business Registration
- Datasets
- Fees
---
