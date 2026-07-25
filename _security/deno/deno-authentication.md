---
api_key_in: []
api_specs:
- filename: deno-apps-api-openapi.yml
  format: yaml
  label: Deno Apps API
  slug: deno-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deno/refs/heads/main/openapi/deno-apps-api-openapi.yml
- filename: deno-deployments-api-openapi.yml
  format: yaml
  label: Deno Deployments API
  slug: deno-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deno/refs/heads/main/openapi/deno-deployments-api-openapi.yml
- filename: deno-domains-api-openapi.yml
  format: yaml
  label: Deno Domains API
  slug: deno-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deno/refs/heads/main/openapi/deno-domains-api-openapi.yml
- filename: deno-kv-databases-api-openapi.yml
  format: yaml
  label: Deno KV Databases API
  slug: deno-kv-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deno/refs/heads/main/openapi/deno-kv-databases-api-openapi.yml
- filename: deno-logs-api-openapi.yml
  format: yaml
  label: Deno Logs API
  slug: deno-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deno/refs/heads/main/openapi/deno-logs-api-openapi.yml
- filename: deno-organizations-api-openapi.yml
  format: yaml
  label: Deno Organizations API
  slug: deno-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deno/refs/heads/main/openapi/deno-organizations-api-openapi.yml
- filename: deno-projects-api-openapi.yml
  format: yaml
  label: Deno Projects API
  slug: deno-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deno/refs/heads/main/openapi/deno-projects-api-openapi.yml
- filename: deno-revisions-api-openapi.yml
  format: yaml
  label: Deno Revisions API
  slug: deno-revisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deno/refs/heads/main/openapi/deno-revisions-api-openapi.yml
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
