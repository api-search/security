---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gankdat-com-changes-api-openapi.yml
  format: yaml
  label: gankdat Changes API
  slug: gankdat-com-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gankdat-com/openapi/gankdat-com-changes-api-openapi.yml
- filename: gankdat-com-data-api-openapi.yml
  format: yaml
  label: gankdat Data API
  slug: gankdat-com-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gankdat-com/openapi/gankdat-com-data-api-openapi.yml
- filename: gankdat-com-platform-api-openapi.yml
  format: yaml
  label: gankdat Platform API
  slug: gankdat-com-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gankdat-com/openapi/gankdat-com-platform-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: gankdat Authentication
name_suffix: Authentication
oauth_flows: []
overview: gankdat secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: gankdat
provider_slug: gankdat-com
scheme_count: 1
schemes:
- description: API key created from your account dashboard (sign in at /account), sent as a bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/gankdat-com-openapi.json
  type: http
slug: gankdat-com-authentication
source_filename: gankdat-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: derived\nsource: openapi/gankdat-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key created from your account dashboard (sign in at /account), sent as a\n    bearer token.\n  sources:\n  - openapi/gankdat-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/gankdat-com/authentication/gankdat-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Data
- Government
- United Kingdom
- EU
---
