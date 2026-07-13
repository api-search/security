---
api_key_in: []
api_specs:
- filename: limble-cmms-limble-api-v2.yaml
  format: yaml
  label: Limble API V2
  slug: limble-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/limble-cmms/refs/heads/main/openapi/limble-cmms-limble-api-v2.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Limble Cmms Authentication
name_suffix: Authentication
oauth_flows: []
overview: Limble CMMS secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Limble CMMS
provider_slug: limble-cmms
scheme_count: 1
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/limble-cmms-limble-api-v2.yaml
  type: http
slug: limble-cmms-authentication
source_filename: limble-cmms-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/limble-cmms-limble-api-v2.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/limble-cmms-limble-api-v2.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/limble-cmms/refs/heads/main/authentication/limble-cmms-authentication.yml
summary_line: http · 1 scheme
tags:
- CMMS
- Maintenance Management
- Asset Management
- Manufacturing
- Facility Management
- Work Orders
---
