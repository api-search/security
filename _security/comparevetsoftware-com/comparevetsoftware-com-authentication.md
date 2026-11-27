---
anonymous_access: false
api_key_in: []
api_specs:
- filename: comparevetsoftware-com-enquiry-api-openapi.yml
  format: yaml
  label: Compare Vet Software Enquiry API
  slug: comparevetsoftware-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comparevetsoftware-com/openapi/comparevetsoftware-com-enquiry-api-openapi.yml
- filename: comparevetsoftware-com-guide-api-openapi.yml
  format: yaml
  label: Compare Vet Software Guide API
  slug: comparevetsoftware-com-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comparevetsoftware-com/openapi/comparevetsoftware-com-guide-api-openapi.yml
- filename: comparevetsoftware-com-mcp-api-openapi.yml
  format: yaml
  label: Compare Vet Software MCP API
  slug: comparevetsoftware-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comparevetsoftware-com/openapi/comparevetsoftware-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Compare Vet Software Authentication
name_suffix: Authentication
oauth_flows: []
overview: Compare Vet Software secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Compare Vet Software
provider_slug: comparevetsoftware-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  required: false
  scheme: bearer
  sources:
  - openapi/comparevetsoftware-com-openapi.yml
  - https://comparevetsoftware.com/mcp
  type: http
slug: comparevetsoftware-com-authentication
source_filename: comparevetsoftware-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://comparevetsoftware.com/openapi.json\ndocs: https://comparevetsoftware.com/mcp\nsummary:\n  types:\n  - http\n  optional: true\n  note: 'Every operation declares security [{}, {accessKey: []}], so anonymous calls are accepted. The MCP card at GET https://comparevetsoftware.com/mcp states \"auth\":\"none\" for the MCP endpoint. The provider documents no process for getting an emk_ access key; the 429 description points to \"docs/MCP.md\", and https://comparevetsoftware.com/docs/MCP.md returned 404 on 2026-11-04.'\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  required: false\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/comparevetsoftware-com-openapi.yml\n  - https://comparevetsoftware.com/mcp\n"
source_yaml_url: https://artifacts.apis.io/comparevetsoftware-com/authentication/comparevetsoftware-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Veterinary
- Practice Management Software
- Software Comparison
- Pricing Data
- Datasets
- United Kingdom
- Veterinary Software
---
