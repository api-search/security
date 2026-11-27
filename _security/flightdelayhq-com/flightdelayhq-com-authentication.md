---
anonymous_access: false
api_key_in: []
api_specs:
- filename: flightdelayhq-com-dataset-api-openapi.yml
  format: yaml
  label: FlightDelayHQ Dataset API
  slug: flightdelayhq-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flightdelayhq-com/openapi/flightdelayhq-com-dataset-api-openapi.yml
- filename: flightdelayhq-com-enquiry-api-openapi.yml
  format: yaml
  label: FlightDelayHQ Enquiry API
  slug: flightdelayhq-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flightdelayhq-com/openapi/flightdelayhq-com-enquiry-api-openapi.yml
- filename: flightdelayhq-com-mcp-api-openapi.yml
  format: yaml
  label: FlightDelayHQ MCP API
  slug: flightdelayhq-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flightdelayhq-com/openapi/flightdelayhq-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: FlightDelayHQ Authentication
name_suffix: Authentication
oauth_flows: []
overview: FlightDelayHQ secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FlightDelayHQ
provider_slug: flightdelayhq-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/flightdelayhq-com-openapi.json
  type: http
slug: flightdelayhq-com-authentication
source_filename: flightdelayhq-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/flightdelayhq-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/flightdelayhq-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/flightdelayhq-com/authentication/flightdelayhq-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Aviation
- Compensation
- Legal
- Travel
- Data
---
