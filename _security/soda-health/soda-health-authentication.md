---
api_key_in: []
api_specs:
- filename: soda-health-docs-portal-openapi-original.json
  format: json
  label: Evermore Docs Portal API
  slug: evermore-docs-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-health/refs/heads/main/openapi/soda-health-docs-portal-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Soda Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Soda Health secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Soda Health
provider_slug: soda-health
scheme_count: 1
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/soda-health-docs-portal-openapi-original.json
  type: http
slug: soda-health-authentication
source_filename: soda-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/soda-health-docs-portal-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/soda-health-docs-portal-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soda-health/refs/heads/main/authentication/soda-health-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Healthcare
- Health Benefits
- Medicare Advantage
- Medicaid
- Supplemental Benefits
- Benefits Administration
- Documentation Portal
---
