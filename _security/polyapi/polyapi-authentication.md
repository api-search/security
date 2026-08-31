---
api_key_in: []
api_specs:
- filename: polyapi-api-functions-api-openapi.yml
  format: yaml
  label: PolyAPI API Functions API
  slug: polyapi-api-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polyapi/refs/heads/main/openapi/polyapi-api-functions-api-openapi.yml
- filename: polyapi-assistants-api-openapi.yml
  format: yaml
  label: PolyAPI Assistants API
  slug: polyapi-assistants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polyapi/refs/heads/main/openapi/polyapi-assistants-api-openapi.yml
- filename: polyapi-client-functions-api-openapi.yml
  format: yaml
  label: PolyAPI Client Functions API
  slug: polyapi-client-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polyapi/refs/heads/main/openapi/polyapi-client-functions-api-openapi.yml
- filename: polyapi-environments-api-openapi.yml
  format: yaml
  label: PolyAPI Environments API
  slug: polyapi-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polyapi/refs/heads/main/openapi/polyapi-environments-api-openapi.yml
- filename: polyapi-jobs-api-openapi.yml
  format: yaml
  label: PolyAPI Jobs API
  slug: polyapi-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polyapi/refs/heads/main/openapi/polyapi-jobs-api-openapi.yml
- filename: polyapi-schemas-api-openapi.yml
  format: yaml
  label: PolyAPI Schemas API
  slug: polyapi-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polyapi/refs/heads/main/openapi/polyapi-schemas-api-openapi.yml
- filename: polyapi-server-functions-api-openapi.yml
  format: yaml
  label: PolyAPI Server Functions API
  slug: polyapi-server-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polyapi/refs/heads/main/openapi/polyapi-server-functions-api-openapi.yml
- filename: polyapi-triggers-api-openapi.yml
  format: yaml
  label: PolyAPI Triggers API
  slug: polyapi-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polyapi/refs/heads/main/openapi/polyapi-triggers-api-openapi.yml
- filename: polyapi-variables-api-openapi.yml
  format: yaml
  label: PolyAPI Variables API
  slug: polyapi-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polyapi/refs/heads/main/openapi/polyapi-variables-api-openapi.yml
- filename: polyapi-webhooks-api-openapi.yml
  format: yaml
  label: PolyAPI Webhooks API
  slug: polyapi-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polyapi/refs/heads/main/openapi/polyapi-webhooks-api-openapi.yml
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
- Integration
- Microservices
- Middleware
- Orchestrations
- Pro-Code API Composition
---
