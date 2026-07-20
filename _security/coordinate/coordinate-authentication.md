---
api_key_in:
- header
api_specs:
- filename: coordinate-openapi.yml
  format: yaml
  label: Coordinate REST API
  slug: coordinate-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coordinate/refs/heads/main/openapi/coordinate-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Coordinate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coordinate secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Coordinate
provider_slug: coordinate
scheme_count: 1
schemes:
- description: 'API key sent in a custom `Bearer:` header (note: this is a header named "Bearer", not the standard `Authorization: Bearer` scheme). Create keys in the Coordinate UI under Settings > Integrations > API Keys. The key scopes all requests to its owning vendor.'
  in: header
  name: BearerHeader
  parameter: Bearer
  sources:
  - openapi/coordinate-openapi.yml
  type: apiKey
slug: coordinate-authentication
source_filename: coordinate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/coordinate-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: BearerHeader\n  type: apiKey\n  in: header\n  parameter: Bearer\n  description: 'API key sent in a custom `Bearer:` header (note: this is a header named \"Bearer\",\n    not the standard `Authorization: Bearer` scheme). Create keys in the Coordinate UI under\n    Settings > Integrations > API Keys. The key scopes all requests to its owning vendor.'\n  sources:\n  - openapi/coordinate-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coordinate/refs/heads/main/authentication/coordinate-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Enterprise Saas
- Project Management
- Client Portal
- Client Onboarding
- Professional Services
- Workflow Automation
- Collaboration
- Webhooks
---
