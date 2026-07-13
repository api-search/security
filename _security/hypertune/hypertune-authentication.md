---
api_key_in:
- query
api_specs:
- filename: hypertune-openapi.yml
  format: yaml
  label: Hypertune Flag Evaluation / Config (GraphQL / SDK) API
  slug: hypertune-flag-evaluation-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hypertune/refs/heads/main/openapi/hypertune-openapi.yml
- filename: hypertune-openapi.yml
  format: yaml
  label: Hypertune Edge Config Delivery API
  slug: hypertune-edge-config-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hypertune/refs/heads/main/openapi/hypertune-openapi.yml
- filename: hypertune-openapi.yml
  format: yaml
  label: Hypertune Analytics / Events API
  slug: hypertune-analytics-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hypertune/refs/heads/main/openapi/hypertune-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Hypertune Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hypertune secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hypertune
provider_slug: hypertune
scheme_count: 1
schemes:
- description: URL-encoded Hypertune project token passed as a query parameter.
  in: query
  name: projectToken
  parameter: token
  sources:
  - openapi/hypertune-openapi.yml
  type: apiKey
slug: hypertune-authentication
source_filename: hypertune-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hypertune-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: projectToken\n  type: apiKey\n  in: query\n  parameter: token\n  description: URL-encoded Hypertune project token passed as a query parameter.\n  sources:\n  - openapi/hypertune-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hypertune/refs/heads/main/authentication/hypertune-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Feature Flags
- Experimentation
- A/B Testing
- Analytics
- App Configuration
- GraphQL
- Edge
---
