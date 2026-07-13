---
api_key_in: []
api_specs:
- filename: acuity-brands.json
  format: json
  label: Acuity Brands API
  slug: acuity-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acuity-brands/refs/heads/main/openapi/acuity-brands.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Acuity Brands Authentication
name_suffix: Authentication
oauth_flows: []
overview: acuity-brands secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: acuity-brands
provider_slug: acuity-brands
scheme_count: 1
schemes:
- description: HTTP Basic Auth using numeric User ID as username and API Key as password
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/acuity-brands.json
  type: http
slug: acuity-brands-authentication
source_filename: acuity-brands-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/acuity-brands.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Auth using numeric User ID as username and API Key as password\n  sources:\n  - openapi/acuity-brands.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acuity-brands/refs/heads/main/authentication/acuity-brands-authentication.yml
summary_line: http · 1 scheme
tags:
- Fortune 1000
---
