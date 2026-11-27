---
anonymous_access: false
api_key_in: []
api_specs:
- filename: brokervsadvisor-com-enquiry-api-openapi.yml
  format: yaml
  label: Broker vs Advisor Enquiry API
  slug: brokervsadvisor-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brokervsadvisor-com/openapi/brokervsadvisor-com-enquiry-api-openapi.yml
- filename: brokervsadvisor-com-guide-api-openapi.yml
  format: yaml
  label: Broker vs Advisor Guide API
  slug: brokervsadvisor-com-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brokervsadvisor-com/openapi/brokervsadvisor-com-guide-api-openapi.yml
- filename: brokervsadvisor-com-mcp-api-openapi.yml
  format: yaml
  label: Broker vs Advisor MCP API
  slug: brokervsadvisor-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brokervsadvisor-com/openapi/brokervsadvisor-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Broker vs Advisor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Broker vs Advisor secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Broker vs Advisor
provider_slug: brokervsadvisor-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/brokervsadvisor-com-openapi.json
  type: http
slug: brokervsadvisor-com-authentication
source_filename: brokervsadvisor-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/brokervsadvisor-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/brokervsadvisor-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/brokervsadvisor-com/authentication/brokervsadvisor-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Business
- Finance
- Legal
- Advisory
- M&A
---
