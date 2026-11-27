---
anonymous_access: false
api_key_in: []
api_specs:
- filename: entitysearchhq-com-dataset-api-openapi.yml
  format: yaml
  label: EntitySearch HQ Dataset API
  slug: entitysearchhq-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entitysearchhq-com/openapi/entitysearchhq-com-dataset-api-openapi.yml
- filename: entitysearchhq-com-enquiry-api-openapi.yml
  format: yaml
  label: EntitySearch HQ Enquiry API
  slug: entitysearchhq-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entitysearchhq-com/openapi/entitysearchhq-com-enquiry-api-openapi.yml
- filename: entitysearchhq-com-mcp-api-openapi.yml
  format: yaml
  label: EntitySearch HQ MCP API
  slug: entitysearchhq-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entitysearchhq-com/openapi/entitysearchhq-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: EntitySearch HQ Authentication
name_suffix: Authentication
oauth_flows: []
overview: EntitySearch HQ secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: EntitySearch HQ
provider_slug: entitysearchhq-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/entitysearchhq-com-openapi.json
  type: http
slug: entitysearchhq-com-authentication
source_filename: entitysearchhq-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/entitysearchhq-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/entitysearchhq-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/entitysearchhq-com/authentication/entitysearchhq-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Data
- Government
- US
- Entity Search
- Business
---
