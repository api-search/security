---
anonymous_access: false
api_key_in: []
api_specs:
- filename: equipmentrentalcompare-com-dataset-api-openapi.yml
  format: yaml
  label: Equipment Rental Compare Dataset API
  slug: equipmentrentalcompare-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/equipmentrentalcompare-com/openapi/equipmentrentalcompare-com-dataset-api-openapi.yml
- filename: equipmentrentalcompare-com-enquiry-api-openapi.yml
  format: yaml
  label: Equipment Rental Compare Enquiry API
  slug: equipmentrentalcompare-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/equipmentrentalcompare-com/openapi/equipmentrentalcompare-com-enquiry-api-openapi.yml
- filename: equipmentrentalcompare-com-mcp-api-openapi.yml
  format: yaml
  label: Equipment Rental Compare MCP API
  slug: equipmentrentalcompare-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/equipmentrentalcompare-com/openapi/equipmentrentalcompare-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Equipment Rental Compare Authentication
name_suffix: Authentication
oauth_flows: []
overview: Equipment Rental Compare secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Equipment Rental Compare
provider_slug: equipmentrentalcompare-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/equipmentrentalcompare-com-openapi.json
  type: http
slug: equipmentrentalcompare-com-authentication
source_filename: equipmentrentalcompare-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/equipmentrentalcompare-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/equipmentrentalcompare-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/equipmentrentalcompare-com/authentication/equipmentrentalcompare-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Equipment Rental
- Directory
- US Market
- Machinery
---
