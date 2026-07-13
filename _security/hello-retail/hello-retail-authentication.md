---
api_key_in: []
api_specs:
- filename: hello-retail-openapi.yml
  format: yaml
  label: Hello Retail API
  slug: hello-retail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hello-retail/refs/heads/main/openapi/hello-retail-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hello Retail Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hello Retail secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hello Retail
provider_slug: hello-retail
scheme_count: 1
schemes:
- bearerFormat: API Key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hello-retail-openapi.yml
  type: http
slug: hello-retail-authentication
source_filename: hello-retail-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hello-retail-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  sources:\n  - openapi/hello-retail-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hello-retail/refs/heads/main/authentication/hello-retail-authentication.yml
summary_line: http · 1 scheme
tags:
- E-Commerce
- Personalization
- Product Recommendations
- Retail
---
