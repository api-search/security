---
api_key_in: []
api_specs:
- filename: labvantage-lims-openapi.yml
  format: yaml
  label: LabVantage LIMS API
  slug: labvantage-lims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/labvantage/refs/heads/main/openapi/labvantage-lims-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Labvantage Authentication
name_suffix: Authentication
oauth_flows: []
overview: LabVantage Solutions secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LabVantage Solutions
provider_slug: labvantage
scheme_count: 2
schemes:
- description: HTTP Basic Authentication (username:password)
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/labvantage-lims-openapi.yml
  type: http
- description: Bearer token authentication
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/labvantage-lims-openapi.yml
  type: http
slug: labvantage-authentication
source_filename: labvantage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/labvantage-lims-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication (username:password)\n  sources:\n  - openapi/labvantage-lims-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication\n  sources:\n  - openapi/labvantage-lims-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/labvantage/refs/heads/main/authentication/labvantage-authentication.yml
summary_line: http · 2 schemes
tags:
- Pharma
- Laboratory
- LIMS
- Quality
- GxP
---
