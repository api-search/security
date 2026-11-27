---
anonymous_access: false
api_key_in: []
api_specs:
- filename: comparetradesoftware-com-enquiry-api-openapi.yml
  format: yaml
  label: Compare Trade Software Enquiry API
  slug: comparetradesoftware-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comparetradesoftware-com/openapi/comparetradesoftware-com-enquiry-api-openapi.yml
- filename: comparetradesoftware-com-guide-api-openapi.yml
  format: yaml
  label: Compare Trade Software Guide API
  slug: comparetradesoftware-com-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comparetradesoftware-com/openapi/comparetradesoftware-com-guide-api-openapi.yml
- filename: comparetradesoftware-com-mcp-api-openapi.yml
  format: yaml
  label: Compare Trade Software MCP API
  slug: comparetradesoftware-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comparetradesoftware-com/openapi/comparetradesoftware-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Compare Trade Software Authentication
name_suffix: Authentication
oauth_flows: []
overview: Compare Trade Software secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Compare Trade Software
provider_slug: comparetradesoftware-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/comparetradesoftware-com-openapi.yml
  type: http
slug: comparetradesoftware-com-authentication
source_filename: comparetradesoftware-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/comparetradesoftware-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/comparetradesoftware-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/comparetradesoftware-com/authentication/comparetradesoftware-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Comparison
- Job Management Software
- Trade
- United Kingdom
- Pricing Data
- Datasets
- MCP
---
