---
api_key_in: []
api_specs:
- filename: argus-enterprise-core-openapi.yml
  format: yaml
  label: ARGUS Enterprise Core API
  slug: argus-enterprise-core
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/openapi/argus-enterprise-core-openapi.yml
- filename: argus-enterprise-webhooks-openapi.yml
  format: yaml
  label: ARGUS Enterprise Webhook API
  slug: argus-enterprise-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/openapi/argus-enterprise-webhooks-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Argus Enterprise Authentication
name_suffix: Authentication
oauth_flows: []
overview: ARGUS Enterprise secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 Bearer token obtained from the /auth/token endpoint using client credentials.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/argus-enterprise-core-openapi.yml
  - openapi/argus-enterprise-webhooks-openapi.yml
  type: http
slug: argus-enterprise-authentication
source_filename: argus-enterprise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/argus-enterprise-core-openapi.yml, openapi/argus-enterprise-webhooks-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 Bearer token obtained from the /auth/token endpoint using client credentials.\n  sources:\n  - openapi/argus-enterprise-core-openapi.yml\n  - openapi/argus-enterprise-webhooks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/authentication/argus-enterprise-authentication.yml
summary_line: http · 1 scheme
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
---
