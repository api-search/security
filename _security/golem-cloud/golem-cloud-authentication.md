---
api_key_in: []
api_specs:
- filename: golem-cloud-openapi.yml
  format: yaml
  label: Golem Components API
  slug: components
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/golem-cloud/refs/heads/main/openapi/golem-cloud-openapi.yml
- filename: golem-cloud-openapi.yml
  format: yaml
  label: Golem Workers & Invocation API
  slug: workers-invocation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/golem-cloud/refs/heads/main/openapi/golem-cloud-openapi.yml
- filename: golem-cloud-openapi.yml
  format: yaml
  label: Golem API Definitions & Deployments API
  slug: api-definitions-deployments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/golem-cloud/refs/heads/main/openapi/golem-cloud-openapi.yml
- filename: golem-cloud-openapi.yml
  format: yaml
  label: Golem Plugins API
  slug: plugins
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/golem-cloud/refs/heads/main/openapi/golem-cloud-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Golem Cloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: Golem secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Golem
provider_slug: golem-cloud
scheme_count: 1
schemes:
- description: Bearer token created for your Golem account. Pass it in the Authorization header as `Bearer <token>`.
  name: Token
  scheme: bearer
  sources:
  - openapi/golem-cloud-openapi.yml
  type: http
slug: golem-cloud-authentication
source_filename: golem-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/golem-cloud-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: Token\n  type: http\n  scheme: bearer\n  description: Bearer token created for your Golem account. Pass it in the Authorization header\n    as `Bearer <token>`.\n  sources:\n  - openapi/golem-cloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/golem-cloud/refs/heads/main/authentication/golem-cloud-authentication.yml
summary_line: http · 1 scheme
tags:
- Durable Computing
- Serverless
- WebAssembly
- Workers
- Agents
---
