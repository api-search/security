---
api_key_in: []
api_specs:
- filename: deno-deploy-rest-api-openapi.yml
  format: yaml
  label: Deno Deploy REST API
  slug: deploy-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deno/refs/heads/main/openapi/deno-deploy-rest-api-openapi.yml
- filename: deno-deploy-v2-api-openapi.yml
  format: yaml
  label: Deno Deploy API V2
  slug: deploy-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deno/refs/heads/main/openapi/deno-deploy-v2-api-openapi.yml
- filename: deno-subhosting-api-openapi.yml
  format: yaml
  label: Deno Subhosting API
  slug: subhosting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deno/refs/heads/main/openapi/deno-subhosting-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Deno Authentication
name_suffix: Authentication
oauth_flows: []
overview: Deno secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Deno
provider_slug: deno
scheme_count: 1
schemes:
- description: Bearer token authentication. Generate tokens from the Deno Deploy dashboard under Settings > Access Tokens.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/deno-deploy-rest-api-openapi.yml
  - openapi/deno-deploy-v2-api-openapi.yml
  - openapi/deno-subhosting-api-openapi.yml
  type: http
slug: deno-authentication
source_filename: deno-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/deno-deploy-rest-api-openapi.yml, openapi/deno-deploy-v2-api-openapi.yml, openapi/deno-subhosting-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication. Generate tokens from the Deno Deploy dashboard under\n    Settings > Access Tokens.\n  sources:\n  - openapi/deno-deploy-rest-api-openapi.yml\n  - openapi/deno-deploy-v2-api-openapi.yml\n  - openapi/deno-subhosting-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deno/refs/heads/main/authentication/deno-authentication.yml
summary_line: http · 1 scheme
tags:
- Deployment
- Edge
- JavaScript
- Runtime
- Serverless
- TypeScript
---
