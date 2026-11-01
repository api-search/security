---
anonymous_access: false
api_key_in: []
api_specs:
- filename: damagerestorehq-com-dataset-api-openapi.yml
  format: yaml
  label: damagerestorehq-com Dataset API
  slug: damagerestorehq-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/damagerestorehq-com/openapi/damagerestorehq-com-dataset-api-openapi.yml
- filename: damagerestorehq-com-enquiry-api-openapi.yml
  format: yaml
  label: damagerestorehq-com Enquiry API
  slug: damagerestorehq-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/damagerestorehq-com/openapi/damagerestorehq-com-enquiry-api-openapi.yml
- filename: damagerestorehq-com-entities-api-openapi.yml
  format: yaml
  label: damagerestorehq-com Entities API
  slug: damagerestorehq-com-entities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/damagerestorehq-com/openapi/damagerestorehq-com-entities-api-openapi.yml
- filename: damagerestorehq-com-mcp-api-openapi.yml
  format: yaml
  label: damagerestorehq-com MCP API
  slug: damagerestorehq-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/damagerestorehq-com/openapi/damagerestorehq-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Damagerestorehq Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: damagerestorehq-com secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: damagerestorehq-com
provider_slug: damagerestorehq-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/damagerestorehq-com-openapi.json
  type: http
slug: damagerestorehq-com-authentication
source_filename: damagerestorehq-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/damagerestorehq-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/damagerestorehq-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/damagerestorehq-com/authentication/damagerestorehq-com-authentication.yml
summary_line: http · 1 scheme
tags:
- WaterDamage
- Insurance
- Restoration
- US
- Data
---
