---
api_key_in: []
api_specs:
- filename: traceable-platform-openapi.yml
  format: yaml
  label: Traceable Platform GraphQL API
  slug: traceable-platform-graphql
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traceable/refs/heads/main/openapi/traceable-platform-openapi.yml
- filename: traceable-platform-openapi.yml
  format: yaml
  label: Traceable API Security Platform
  slug: traceable-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traceable/refs/heads/main/openapi/traceable-platform-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Traceable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Traceable secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Traceable
provider_slug: traceable
scheme_count: 1
schemes:
- description: Platform API token generated through the Traceable dashboard. Pass as a Bearer token in the Authorization header. Tokens are single-use and cannot be retrieved after initial generation.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/traceable-platform-openapi.yml
  type: http
slug: traceable-authentication
source_filename: traceable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/traceable-platform-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Platform API token generated through the Traceable dashboard. Pass as a Bearer\n    token in the Authorization header. Tokens are single-use and cannot be retrieved after initial\n    generation.\n  sources:\n  - openapi/traceable-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/traceable/refs/heads/main/authentication/traceable-authentication.yml
summary_line: http · 1 scheme
tags:
- API Discovery
- API Protection
- API Security
- API Testing
- Observability
- Security
- Threat Detection
---
