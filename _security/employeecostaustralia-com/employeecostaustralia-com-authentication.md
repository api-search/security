---
anonymous_access: false
api_key_in: []
api_specs:
- filename: employeecostaustralia-com-calculator-api-openapi.yml
  format: yaml
  label: Employee Cost Australia Calculator API
  slug: employeecostaustralia-com-calculator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/employeecostaustralia-com/openapi/employeecostaustralia-com-calculator-api-openapi.yml
- filename: employeecostaustralia-com-enquiry-api-openapi.yml
  format: yaml
  label: Employee Cost Australia Enquiry API
  slug: employeecostaustralia-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/employeecostaustralia-com/openapi/employeecostaustralia-com-enquiry-api-openapi.yml
- filename: employeecostaustralia-com-mcp-api-openapi.yml
  format: yaml
  label: Employee Cost Australia MCP API
  slug: employeecostaustralia-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/employeecostaustralia-com/openapi/employeecostaustralia-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Employee Cost Australia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Employee Cost Australia secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Employee Cost Australia
provider_slug: employeecostaustralia-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/employeecostaustralia-com-openapi.json
  type: http
slug: employeecostaustralia-com-authentication
source_filename: employeecostaustralia-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/employeecostaustralia-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/employeecostaustralia-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/employeecostaustralia-com/authentication/employeecostaustralia-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Employee Cost Calculator
- Superannuation
- Payroll Tax
- Workers Compensation
- Australian Employers
---
