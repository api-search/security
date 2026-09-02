---
api_key_in:
- header
api_specs:
- filename: eppo-allocations-api-openapi.yml
  format: yaml
  label: Eppo Allocations API
  slug: eppo-allocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eppo/refs/heads/main/openapi/eppo-allocations-api-openapi.yml
- filename: eppo-assignments-api-openapi.yml
  format: yaml
  label: Eppo Assignments API
  slug: eppo-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eppo/refs/heads/main/openapi/eppo-assignments-api-openapi.yml
- filename: eppo-experiments-api-openapi.yml
  format: yaml
  label: Eppo Experiments API
  slug: eppo-experiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eppo/refs/heads/main/openapi/eppo-experiments-api-openapi.yml
- filename: eppo-flags-api-openapi.yml
  format: yaml
  label: Eppo Flags API
  slug: eppo-flags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eppo/refs/heads/main/openapi/eppo-flags-api-openapi.yml
- filename: eppo-metrics-api-openapi.yml
  format: yaml
  label: Eppo Metrics API
  slug: eppo-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eppo/refs/heads/main/openapi/eppo-metrics-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Eppo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eppo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Eppo
provider_slug: eppo
scheme_count: 1
schemes:
- description: Eppo REST API key created in Admin > API Keys. Distinct from Eppo SDK keys used to connect SDK clients.
  in: header
  name: eppoToken
  parameter: X-Eppo-Token
  sources:
  - openapi/eppo-openapi.yml
  type: apiKey
slug: eppo-authentication
source_filename: eppo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/eppo-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: eppoToken\n  type: apiKey\n  in: header\n  parameter: X-Eppo-Token\n  description: Eppo REST API key created in Admin > API Keys. Distinct from Eppo SDK keys used\n    to connect SDK clients.\n  sources:\n  - openapi/eppo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eppo/refs/heads/main/authentication/eppo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Experimentation
- Feature Flags
- A/B Testing
- Analytics
- Statistics
---
