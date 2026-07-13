---
api_key_in: []
api_specs:
- filename: florist-one-openapi.yml
  format: yaml
  label: Florist One API
  slug: florist-one-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/florist-one/refs/heads/main/openapi/florist-one-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Florist One Authentication
name_suffix: Authentication
oauth_flows: []
overview: Florist One secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Florist One
provider_slug: florist-one
scheme_count: 1
schemes:
- description: HTTP Basic auth with API Key as username and assigned password
  name: basicAuth
  scheme: basic
  sources:
  - openapi/florist-one-openapi.yml
  type: http
slug: florist-one-authentication
source_filename: florist-one-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/florist-one-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth with API Key as username and assigned password\n  sources:\n  - openapi/florist-one-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/florist-one/refs/heads/main/authentication/florist-one-authentication.yml
summary_line: http · 1 scheme
tags:
- Delivery
- Ecommerce
- Florists
- Flowers
- Gifts
---
