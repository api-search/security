---
anonymous_access: false
api_key_in: []
api_specs:
- filename: eligiblebydescent-com-enquiry-api-openapi.yml
  format: yaml
  label: Eligible By Descent Enquiry API
  slug: eligiblebydescent-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eligiblebydescent-com/openapi/eligiblebydescent-com-enquiry-api-openapi.yml
- filename: eligiblebydescent-com-guide-api-openapi.yml
  format: yaml
  label: Eligible By Descent Guide API
  slug: eligiblebydescent-com-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eligiblebydescent-com/openapi/eligiblebydescent-com-guide-api-openapi.yml
- filename: eligiblebydescent-com-mcp-api-openapi.yml
  format: yaml
  label: Eligible By Descent MCP API
  slug: eligiblebydescent-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eligiblebydescent-com/openapi/eligiblebydescent-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Eligible By Descent Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eligible By Descent secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Eligible By Descent
provider_slug: eligiblebydescent-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/eligiblebydescent-com-openapi.json
  type: http
slug: eligiblebydescent-com-authentication
source_filename: eligiblebydescent-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/eligiblebydescent-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/eligiblebydescent-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/eligiblebydescent-com/authentication/eligiblebydescent-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Citizenship
- Portugal
- Descent
- Guidance
---
