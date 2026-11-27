---
anonymous_access: false
api_key_in: []
api_specs:
- filename: open-factory-com-free-api-openapi.yml
  format: yaml
  label: Open Factory Free API
  slug: open-factory-com-free-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/open-factory-com/openapi/open-factory-com-free-api-openapi.yml
- filename: open-factory-com-institutional-api-openapi.yml
  format: yaml
  label: Open Factory Institutional API
  slug: open-factory-com-institutional-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/open-factory-com/openapi/open-factory-com-institutional-api-openapi.yml
- filename: open-factory-com-pro-api-openapi.yml
  format: yaml
  label: Open Factory Pro API
  slug: open-factory-com-pro-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/open-factory-com/openapi/open-factory-com-pro-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Open Factory Authentication
name_suffix: Authentication
oauth_flows: []
overview: Open Factory secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Open Factory
provider_slug: open-factory-com
scheme_count: 1
schemes:
- description: API key from the docs page. Optional on free endpoints.
  name: bearer
  scheme: bearer
  sources:
  - openapi/open-factory-com-openapi.json
  type: http
slug: open-factory-com-authentication
source_filename: open-factory-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: derived\nsource: openapi/open-factory-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: API key from the docs page. Optional on free endpoints.\n  sources:\n  - openapi/open-factory-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/open-factory-com/authentication/open-factory-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Data
- Research
- Manufacturing
- Data Center
- Equipment
---
