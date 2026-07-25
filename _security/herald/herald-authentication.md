---
api_key_in: []
api_specs:
- filename: herald-applications-api-openapi.yml
  format: yaml
  label: Herald Applications API
  slug: herald-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/herald/refs/heads/main/openapi/herald-applications-api-openapi.yml
- filename: herald-authentication-api-openapi.yml
  format: yaml
  label: Herald Authentication API
  slug: herald-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/herald/refs/heads/main/openapi/herald-authentication-api-openapi.yml
- filename: herald-classifications-api-openapi.yml
  format: yaml
  label: Herald Classifications API
  slug: herald-classifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/herald/refs/heads/main/openapi/herald-classifications-api-openapi.yml
- filename: herald-distributors-api-openapi.yml
  format: yaml
  label: Herald Distributors API
  slug: herald-distributors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/herald/refs/heads/main/openapi/herald-distributors-api-openapi.yml
- filename: herald-files-api-openapi.yml
  format: yaml
  label: Herald Files API
  slug: herald-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/herald/refs/heads/main/openapi/herald-files-api-openapi.yml
- filename: herald-producers-api-openapi.yml
  format: yaml
  label: Herald Producers API
  slug: herald-producers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/herald/refs/heads/main/openapi/herald-producers-api-openapi.yml
- filename: herald-products-api-openapi.yml
  format: yaml
  label: Herald Products API
  slug: herald-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/herald/refs/heads/main/openapi/herald-products-api-openapi.yml
- filename: herald-quotes-api-openapi.yml
  format: yaml
  label: Herald Quotes API
  slug: herald-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/herald/refs/heads/main/openapi/herald-quotes-api-openapi.yml
- filename: herald-submissions-api-openapi.yml
  format: yaml
  label: Herald Submissions API
  slug: herald-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/herald/refs/heads/main/openapi/herald-submissions-api-openapi.yml
- filename: herald-webhooks-api-openapi.yml
  format: yaml
  label: Herald Webhooks API
  slug: herald-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/herald/refs/heads/main/openapi/herald-webhooks-api-openapi.yml
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
