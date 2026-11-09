---
anonymous_access: false
api_key_in: []
api_specs:
- filename: caspchecklist-com-enquiry-api-openapi.yml
  format: yaml
  label: CASP Checklist Enquiry API
  slug: caspchecklist-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caspchecklist-com/openapi/caspchecklist-com-enquiry-api-openapi.yml
- filename: caspchecklist-com-guide-api-openapi.yml
  format: yaml
  label: CASP Checklist Guide API
  slug: caspchecklist-com-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caspchecklist-com/openapi/caspchecklist-com-guide-api-openapi.yml
- filename: caspchecklist-com-mcp-api-openapi.yml
  format: yaml
  label: CASP Checklist MCP API
  slug: caspchecklist-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caspchecklist-com/openapi/caspchecklist-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Caspchecklist Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: CASP Checklist secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CASP Checklist
provider_slug: caspchecklist-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/caspchecklist-com-openapi.json
  type: http
slug: caspchecklist-com-authentication
source_filename: caspchecklist-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/caspchecklist-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/caspchecklist-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/caspchecklist-com/authentication/caspchecklist-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Cryptocurrency
- EU
- MiCA
- Compliance
---
