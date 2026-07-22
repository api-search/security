---
api_key_in:
- header
api_specs:
- filename: remberg-assets-openapi.json
  format: json
  label: remberg Assets API
  slug: remberg-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-assets-openapi.json
- filename: remberg-work-orders-openapi.json
  format: json
  label: remberg Work Orders API
  slug: remberg-work-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-work-orders-openapi.json
- filename: remberg-work-requests-openapi.json
  format: json
  label: remberg Work Requests API
  slug: remberg-work-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-work-requests-openapi.json
- filename: remberg-tickets-openapi.json
  format: json
  label: remberg Tickets API
  slug: remberg-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-tickets-openapi.json
- filename: remberg-parts-openapi.json
  format: json
  label: remberg Parts API
  slug: remberg-parts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-parts-openapi.json
- filename: remberg-organizations-openapi.json
  format: json
  label: remberg Organizations API
  slug: remberg-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-organizations-openapi.json
- filename: remberg-contacts-openapi.json
  format: json
  label: remberg Contacts API
  slug: remberg-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-contacts-openapi.json
- filename: remberg-users-openapi.json
  format: json
  label: remberg Users API
  slug: remberg-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-users-openapi.json
- filename: remberg-files-openapi.json
  format: json
  label: remberg Files API
  slug: remberg-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-files-openapi.json
- filename: remberg-forms-openapi.json
  format: json
  label: remberg Forms API
  slug: remberg-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-forms-openapi.json
- filename: remberg-procedures-openapi.json
  format: json
  label: remberg Procedures API
  slug: remberg-procedures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-procedures-openapi.json
- filename: remberg-ai-openapi.json
  format: json
  label: remberg AI Copilot API
  slug: remberg-ai-copilot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-ai-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Remberg Authentication
name_suffix: Authentication
oauth_flows: []
overview: Remberg secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Remberg
provider_slug: remberg
scheme_count: 1
schemes:
- in: header
  name: authorization
  parameter: authorization
  sources:
  - openapi/remberg-ai-openapi.json
  - openapi/remberg-assets-openapi.json
  - openapi/remberg-contacts-openapi.json
  - openapi/remberg-files-openapi.json
  - openapi/remberg-forms-openapi.json
  - openapi/remberg-organizations-openapi.json
  - openapi/remberg-parts-openapi.json
  - openapi/remberg-procedures-openapi.json
  - openapi/remberg-tickets-openapi.json
  - openapi/remberg-users-openapi.json
  - openapi/remberg-work-orders-openapi.json
  - openapi/remberg-work-requests-openapi.json
  type: apiKey
slug: remberg-authentication
source_filename: remberg-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/remberg-ai-openapi.json, openapi/remberg-assets-openapi.json, openapi/remberg-contacts-openapi.json,\n  openapi/remberg-files-openapi.json, openapi/remberg-forms-openapi.json, openapi/remberg-organizations-openapi.json,\n  openapi/remberg-parts-openapi.json, openapi/remberg-procedures-openapi.json, openapi/remberg-tickets-openapi.json,\n  openapi/remberg-users-openapi.json, openapi/remberg-work-orders-openapi.json, openapi/remberg-work-requests-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: authorization\n  type: apiKey\n  in: header\n  parameter: authorization\n  sources:\n  - openapi/remberg-ai-openapi.json\n  - openapi/remberg-assets-openapi.json\n  - openapi/remberg-contacts-openapi.json\n  - openapi/remberg-files-openapi.json\n  - openapi/remberg-forms-openapi.json\n  - openapi/remberg-organizations-openapi.json\n  - openapi/remberg-parts-openapi.json\n  - openapi/remberg-procedures-openapi.json\n\
  \  - openapi/remberg-tickets-openapi.json\n  - openapi/remberg-users-openapi.json\n  - openapi/remberg-work-orders-openapi.json\n  - openapi/remberg-work-requests-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/authentication/remberg-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Maintenance
- Asset Management
- CMMS
- EAM
- Field Service
- Work Orders
- Industrial
- SaaS
- Germany
---
