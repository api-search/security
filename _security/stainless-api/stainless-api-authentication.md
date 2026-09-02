---
api_key_in: []
api_specs:
- filename: stainless-api-build-target-outputs-api-openapi.yml
  format: yaml
  label: Stainless Build Target Outputs API
  slug: stainless-api-build-target-outputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stainless-api/refs/heads/main/openapi/stainless-api-build-target-outputs-api-openapi.yml
- filename: stainless-api-builds-api-openapi.yml
  format: yaml
  label: Stainless Builds API
  slug: stainless-api-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stainless-api/refs/heads/main/openapi/stainless-api-builds-api-openapi.yml
- filename: stainless-api-orgs-api-openapi.yml
  format: yaml
  label: Stainless Orgs API
  slug: stainless-api-orgs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stainless-api/refs/heads/main/openapi/stainless-api-orgs-api-openapi.yml
- filename: stainless-api-projects-api-openapi.yml
  format: yaml
  label: Stainless Projects API
  slug: stainless-api-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stainless-api/refs/heads/main/openapi/stainless-api-projects-api-openapi.yml
- filename: stainless-api-user-api-openapi.yml
  format: yaml
  label: Stainless User API
  slug: stainless-api-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stainless-api/refs/heads/main/openapi/stainless-api-user-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Stainless Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stainless secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Stainless
provider_slug: stainless-api
scheme_count: 1
schemes:
- bearerFormat: API Key
  description: Stainless API key passed as a Bearer token.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/stainless-api-openapi.yml
  type: http
slug: stainless-api-authentication
source_filename: stainless-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stainless-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: Stainless API key passed as a Bearer token.\n  sources:\n  - openapi/stainless-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stainless-api/refs/heads/main/authentication/stainless-api-authentication.yml
summary_line: http · 1 scheme
tags:
- SDK Generation
- OpenAPI
- API Tooling
- Developer Experience
- MCP
- Documentation
- Code Generation
- Terraform Provider
- API Reference
- DevTools
- API-First
---
