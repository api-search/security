---
anonymous_access: false
api_key_in: []
api_specs:
- filename: businessvaluenow-com-enquiry-api-openapi.yml
  format: yaml
  label: Business Value Now Enquiry API
  slug: businessvaluenow-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessvaluenow-com/openapi/businessvaluenow-com-enquiry-api-openapi.yml
- filename: businessvaluenow-com-guide-api-openapi.yml
  format: yaml
  label: Business Value Now Guide API
  slug: businessvaluenow-com-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessvaluenow-com/openapi/businessvaluenow-com-guide-api-openapi.yml
- filename: businessvaluenow-com-mcp-api-openapi.yml
  format: yaml
  label: Business Value Now MCP API
  slug: businessvaluenow-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessvaluenow-com/openapi/businessvaluenow-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Business Value Now Authentication
name_suffix: Authentication
oauth_flows: []
overview: Business Value Now secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Business Value Now
provider_slug: businessvaluenow-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/businessvaluenow-com-openapi.json
  type: http
slug: businessvaluenow-com-authentication
source_filename: businessvaluenow-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/businessvaluenow-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/businessvaluenow-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/businessvaluenow-com/authentication/businessvaluenow-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Business Valuation
- Finance
- Education
- Entrepreneurship
- Small Business
---
