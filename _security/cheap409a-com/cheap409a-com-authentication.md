---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cheap409a-com-enquiry-api-openapi.yml
  format: yaml
  label: Cheap 409A Enquiry API
  slug: cheap409a-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cheap409a-com/openapi/cheap409a-com-enquiry-api-openapi.yml
- filename: cheap409a-com-guide-api-openapi.yml
  format: yaml
  label: Cheap 409A Guide API
  slug: cheap409a-com-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cheap409a-com/openapi/cheap409a-com-guide-api-openapi.yml
- filename: cheap409a-com-mcp-api-openapi.yml
  format: yaml
  label: Cheap 409A MCP API
  slug: cheap409a-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cheap409a-com/openapi/cheap409a-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Cheap 409A Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cheap 409A secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cheap 409A
provider_slug: cheap409a-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/cheap409a-com-original.json
  type: http
slug: cheap409a-com-authentication
source_filename: cheap409a-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/cheap409a-com-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/cheap409a-com-original.json\n"
source_yaml_url: https://artifacts.apis.io/cheap409a-com/authentication/cheap409a-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Valuation
- Startups
- Finance
- Pricing
---
