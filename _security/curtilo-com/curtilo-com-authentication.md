---
anonymous_access: false
api_key_in: []
api_specs:
- filename: curtilo-com-dataset-api-openapi.yml
  format: yaml
  label: Curtilo Dataset API
  slug: curtilo-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/curtilo-com/openapi/curtilo-com-dataset-api-openapi.yml
- filename: curtilo-com-mcp-api-openapi.yml
  format: yaml
  label: Curtilo MCP API
  slug: curtilo-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/curtilo-com/openapi/curtilo-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Curtilo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Curtilo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Curtilo
provider_slug: curtilo-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/curtilo-com-openapi.yml
  type: http
slug: curtilo-com-authentication
source_filename: curtilo-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/curtilo-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/curtilo-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/curtilo-com/authentication/curtilo-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Planning
- Permitted Development
- Property Development
- Land Sourcing
- Real Estate
- United Kingdom
- Datasets
---
