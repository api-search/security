---
api_key_in: []
api_specs:
- filename: oracle-health-data-intelligence-openapi.yml
  format: yaml
  label: Oracle Health Data Intelligence
  slug: oracle-health-data-intelligence
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-health-data-intelligence/refs/heads/main/openapi/oracle-health-data-intelligence-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Oracle Health Data Intelligence Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oracle Health Data Intelligence secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Oracle Health Data Intelligence
provider_slug: oracle-health-data-intelligence
scheme_count: 1
schemes:
- description: Bearer token supplied via the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/oracle-health-data-intelligence-openapi.yml
  type: http
slug: oracle-health-data-intelligence-authentication
source_filename: oracle-health-data-intelligence-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oracle-health-data-intelligence-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token supplied via the Authorization header.\n  sources:\n  - openapi/oracle-health-data-intelligence-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-health-data-intelligence/refs/heads/main/authentication/oracle-health-data-intelligence-authentication.yml
summary_line: http · 1 scheme
tags:
- Genomic
- Health Records
- Healthcare
---
