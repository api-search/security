---
anonymous_access: false
api_key_in: []
api_specs:
- filename: accountancyvaluation-com-enquiry-api-openapi.yml
  format: yaml
  label: Accountancy Valuation Enquiry API
  slug: accountancyvaluation-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/accountancyvaluation-com/openapi/accountancyvaluation-com-enquiry-api-openapi.yml
- filename: accountancyvaluation-com-mcp-api-openapi.yml
  format: yaml
  label: Accountancy Valuation MCP API
  slug: accountancyvaluation-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/accountancyvaluation-com/openapi/accountancyvaluation-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Accountancyvaluation Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Accountancy Valuation secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Accountancy Valuation
provider_slug: accountancyvaluation-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/accountancyvaluation-com-openapi.yml
  - openapi/openapi.json
  type: http
slug: accountancyvaluation-com-authentication
source_filename: accountancyvaluation-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/accountancyvaluation-com-openapi.yml, openapi/openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/accountancyvaluation-com-openapi.yml\n  - openapi/openapi.json\n"
source_yaml_url: https://artifacts.apis.io/accountancyvaluation-com/authentication/accountancyvaluation-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Accounting
- Valuation
- CPA
- Practice
- US
---
