---
api_key_in: []
api_specs:
- filename: zoominfo-openapi.yml
  format: yaml
  label: ZoomInfo
  slug: zoominfo
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/openapi/zoominfo-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Zoominfo Authentication
name_suffix: Authentication
oauth_flows: []
overview: ZoomInfo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ZoomInfo
provider_slug: zoominfo
scheme_count: 1
schemes:
- name: httpBearer
  scheme: bearer
  sources:
  - openapi/zoominfo-openapi.yml
  type: http
slug: zoominfo-authentication
source_filename: zoominfo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zoominfo-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: httpBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/zoominfo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/authentication/zoominfo-authentication.yml
summary_line: http · 1 scheme
tags:
- B2B
- B2B Data
- Company Data
- Contact Database
- Contacts
- Data
- Lead Generation
- Marketing Intelligence
- Sales Intelligence
---
