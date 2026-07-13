---
api_key_in: []
api_specs:
- filename: tango-raas-api-openapi.yml
  format: yaml
  label: Tango RaaS API
  slug: raas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango/refs/heads/main/openapi/tango-raas-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tango Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tango secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tango
provider_slug: tango
scheme_count: 1
schemes:
- description: HTTP Basic Auth using platform credentials (username/password)
  name: basicAuth
  scheme: basic
  sources:
  - openapi/tango-raas-api-openapi.yml
  type: http
slug: tango-authentication
source_filename: tango-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tango-raas-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Auth using platform credentials (username/password)\n  sources:\n  - openapi/tango-raas-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tango/refs/heads/main/authentication/tango-authentication.yml
summary_line: http · 1 scheme
tags:
- Catalog Management
- Digital Rewards
- Gift Cards
- Incentives
- Loyalty
- Rewards As A Service
---
