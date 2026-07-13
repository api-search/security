---
api_key_in: []
api_specs:
- filename: goatcounter-openapi.yml
  format: yaml
  label: GoatCounter
  slug: goatcounter
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/openapi/goatcounter-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Goatcounter Authentication
name_suffix: Authentication
oauth_flows: []
overview: GoatCounter secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GoatCounter
provider_slug: goatcounter
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/goatcounter-openapi.yml
  type: http
slug: goatcounter-authentication
source_filename: goatcounter-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/goatcounter-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/goatcounter-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/authentication/goatcounter-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics
- Pageviews
- Privacy
- Statistics
- Web Analytics
---
