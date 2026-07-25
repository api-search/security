---
api_key_in: []
api_specs:
- filename: goatcounter-exports-api-openapi.yml
  format: yaml
  label: GoatCounter Exports API
  slug: goatcounter-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/openapi/goatcounter-exports-api-openapi.yml
- filename: goatcounter-pageviews-api-openapi.yml
  format: yaml
  label: GoatCounter Pageviews API
  slug: goatcounter-pageviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/openapi/goatcounter-pageviews-api-openapi.yml
- filename: goatcounter-paths-api-openapi.yml
  format: yaml
  label: GoatCounter Paths API
  slug: goatcounter-paths-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/openapi/goatcounter-paths-api-openapi.yml
- filename: goatcounter-sites-api-openapi.yml
  format: yaml
  label: GoatCounter Sites API
  slug: goatcounter-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/openapi/goatcounter-sites-api-openapi.yml
- filename: goatcounter-statistics-api-openapi.yml
  format: yaml
  label: GoatCounter Statistics API
  slug: goatcounter-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/openapi/goatcounter-statistics-api-openapi.yml
- filename: goatcounter-users-api-openapi.yml
  format: yaml
  label: GoatCounter Users API
  slug: goatcounter-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/openapi/goatcounter-users-api-openapi.yml
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
