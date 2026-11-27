---
anonymous_access: false
api_key_in: []
api_specs:
- filename: eseo-su-openapi.yml
  format: yaml
  label: ESEO Public API
  slug: eseo-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eseo-su/openapi/eseo-su-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: ESEO Authentication
name_suffix: Authentication
oauth_flows: []
overview: ESEO secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ESEO
provider_slug: eseo-su
scheme_count: 1
schemes:
- bearerFormat: eseo_token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/eseo-su-openapi.json
  type: http
slug: eseo-su-authentication
source_filename: eseo-su-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/eseo-su-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: eseo_token\n  sources:\n  - openapi/eseo-su-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/eseo-su/authentication/eseo-su-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- E-Commerce
- SEO
- Marketplace
- Automation
- Company
---
