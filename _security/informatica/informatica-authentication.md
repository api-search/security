---
api_key_in:
- header
api_specs:
- filename: informatica-platform-rest-api-openapi.yml
  format: yaml
  label: Informatica Platform REST API
  slug: informatica
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/informatica/refs/heads/main/openapi/informatica-platform-rest-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Informatica Authentication
name_suffix: Authentication
oauth_flows: []
overview: Informatica secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Informatica
provider_slug: informatica
scheme_count: 1
schemes:
- description: The REST API session ID returned by the login endpoint. Include this value in the icSessionId header for all authenticated requests. The session expires after 30 minutes of inactivity.
  in: header
  name: icSessionId
  parameter: icSessionId
  sources:
  - openapi/informatica-platform-rest-api-openapi.yml
  type: apiKey
slug: informatica-authentication
source_filename: informatica-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/informatica-platform-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: icSessionId\n  type: apiKey\n  in: header\n  parameter: icSessionId\n  description: The REST API session ID returned by the login endpoint. Include this value in\n    the icSessionId header for all authenticated requests. The session expires after 30 minutes\n    of inactivity.\n  sources:\n  - openapi/informatica-platform-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/informatica/refs/heads/main/authentication/informatica-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Address Verification
- B2B Gateway
- Cloud Services
- Data Governance
- Data Integration
- Data Profiling
- Data Quality
- Enterprise Software
- ETL
- IDMC
- IICS
- Master Data Management
- Reference Data Management
---
