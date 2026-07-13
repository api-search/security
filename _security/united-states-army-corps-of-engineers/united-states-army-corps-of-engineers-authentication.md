---
api_key_in: []
api_specs:
- filename: cwms-data-api-openapi.yml
  format: yaml
  label: CWMS Data API
  slug: cwms-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-army-corps-of-engineers/refs/heads/main/openapi/cwms-data-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: United States Army Corps Of Engineers Authentication
name_suffix: Authentication
oauth_flows: []
overview: United States Army Corps of Engineers secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: United States Army Corps of Engineers
provider_slug: united-states-army-corps-of-engineers
scheme_count: 1
schemes:
- description: JWT Bearer token for authenticated operations (create, update, delete). Obtain a token from the CWMS authorization endpoint.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cwms-data-api-openapi.yml
  type: http
slug: united-states-army-corps-of-engineers-authentication
source_filename: united-states-army-corps-of-engineers-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cwms-data-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: JWT Bearer token for authenticated operations (create, update, delete). Obtain\n    a token from the CWMS authorization endpoint.\n  sources:\n  - openapi/cwms-data-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-states-army-corps-of-engineers/refs/heads/main/authentication/united-states-army-corps-of-engineers-authentication.yml
summary_line: http · 1 scheme
tags:
- Engineering
- Federal Government
- Water Resources
- Hydrology
- Civil Engineering
---
