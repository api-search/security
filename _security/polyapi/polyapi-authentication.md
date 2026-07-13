---
api_key_in: []
api_specs:
- filename: polyapi-platform-openapi.yml
  format: yaml
  label: PolyAPI Platform API
  slug: polyapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polyapi/refs/heads/main/openapi/polyapi-platform-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Polyapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: PolyAPI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PolyAPI
provider_slug: polyapi
scheme_count: 1
schemes:
- bearerFormat: API Key
  description: PolyAPI uses Bearer token authentication. Include your API key in the Authorization header as 'Bearer {your-api-key}'.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/polyapi-platform-openapi.yml
  type: http
slug: polyapi-authentication
source_filename: polyapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/polyapi-platform-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: PolyAPI uses Bearer token authentication. Include your API key in the Authorization\n    header as 'Bearer {your-api-key}'.\n  sources:\n  - openapi/polyapi-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polyapi/refs/heads/main/authentication/polyapi-authentication.yml
summary_line: http · 1 scheme
tags:
- Integrations
- Microservices
- Middleware
- Orchestrations
- Pro-Code API Composition
---
