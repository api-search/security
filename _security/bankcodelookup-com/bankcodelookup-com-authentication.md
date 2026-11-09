---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bankcodelookup-com-dataset-api-openapi.yml
  format: yaml
  label: Bank Code Lookup Dataset API
  slug: bankcodelookup-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankcodelookup-com/openapi/bankcodelookup-com-dataset-api-openapi.yml
- filename: bankcodelookup-com-enquiry-api-openapi.yml
  format: yaml
  label: Bank Code Lookup Enquiry API
  slug: bankcodelookup-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankcodelookup-com/openapi/bankcodelookup-com-enquiry-api-openapi.yml
- filename: bankcodelookup-com-mcp-api-openapi.yml
  format: yaml
  label: Bank Code Lookup MCP API
  slug: bankcodelookup-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankcodelookup-com/openapi/bankcodelookup-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Bankcodelookup Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bank Code Lookup secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bank Code Lookup
provider_slug: bankcodelookup-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/bankcodelookup-com-openapi.json
  type: http
slug: bankcodelookup-com-authentication
source_filename: bankcodelookup-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/bankcodelookup-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/bankcodelookup-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/bankcodelookup-com/authentication/bankcodelookup-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Banking
- Finance
- Lookup
- Codes
---
