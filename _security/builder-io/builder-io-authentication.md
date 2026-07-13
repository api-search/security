---
api_key_in:
- query
api_specs:
- filename: builder-io-content-api-openapi.yml
  format: yaml
  label: Builder.io Content API
  slug: content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builder-io/refs/heads/main/openapi/builder-io-content-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Builder Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Builder.io secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Builder.io
provider_slug: builder-io
scheme_count: 1
schemes:
- description: Public API key for your Builder.io space.
  in: query
  name: apiKeyQuery
  parameter: apiKey
  sources:
  - openapi/builder-io-content-api-openapi.yml
  type: apiKey
slug: builder-io-authentication
source_filename: builder-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/builder-io-content-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: Public API key for your Builder.io space.\n  sources:\n  - openapi/builder-io-content-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/builder-io/refs/heads/main/authentication/builder-io-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Headless CMS
- Visual Development
- Content Delivery
- A/B Testing
- GraphQL
- REST
- Personalization
- Page Building
---
