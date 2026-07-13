---
api_key_in: []
api_specs:
- filename: herald-openapi.yml
  format: yaml
  label: Herald Applications API
  slug: applications
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/herald/refs/heads/main/openapi/herald-openapi.yml
- filename: herald-openapi.yml
  format: yaml
  label: Herald Quotes API
  slug: quotes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/herald/refs/heads/main/openapi/herald-openapi.yml
- filename: herald-openapi.yml
  format: yaml
  label: Herald Products API
  slug: products
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/herald/refs/heads/main/openapi/herald-openapi.yml
- filename: herald-openapi.yml
  format: yaml
  label: Herald Classifications API
  slug: classifications
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/herald/refs/heads/main/openapi/herald-openapi.yml
- filename: herald-openapi.yml
  format: yaml
  label: Herald Distributors API
  slug: distributors
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/herald/refs/heads/main/openapi/herald-openapi.yml
- filename: herald-openapi.yml
  format: yaml
  label: Herald Files API
  slug: files
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/herald/refs/heads/main/openapi/herald-openapi.yml
- filename: herald-openapi.yml
  format: yaml
  label: Herald Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/herald/refs/heads/main/openapi/herald-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Herald Authentication
name_suffix: Authentication
oauth_flows: []
overview: Herald secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Herald
provider_slug: herald
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Send an API key or an access token from /auth/token in the Authorization header as `Bearer <token>`. Access tokens are obtained via the OAuth2 client-credentials grant and expire after 24 hours.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/herald-openapi.yml
  type: http
slug: herald-authentication
source_filename: herald-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/herald-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Send an API key or an access token from /auth/token in the Authorization header\n    as `Bearer <token>`. Access tokens are obtained via the OAuth2 client-credentials grant\n    and expire after 24 hours.\n  sources:\n  - openapi/herald-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/herald/refs/heads/main/authentication/herald-authentication.yml
summary_line: http · 1 scheme
tags:
- Insurance
- Insurtech
- Commercial Insurance
- Quoting
- Carriers
---
