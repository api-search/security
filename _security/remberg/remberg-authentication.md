---
api_key_in:
- header
api_specs:
- filename: remberg-ai-chat-api-openapi.yml
  format: yaml
  label: Remberg ai-chat API
  slug: remberg-ai-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-ai-chat-api-openapi.yml
- filename: remberg-asset-status-signals-api-openapi.yml
  format: yaml
  label: Remberg asset-status-signals API
  slug: remberg-asset-status-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-asset-status-signals-api-openapi.yml
- filename: remberg-asset-types-api-openapi.yml
  format: yaml
  label: Remberg asset-types API
  slug: remberg-asset-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-asset-types-api-openapi.yml
- filename: remberg-assets-api-openapi.yml
  format: yaml
  label: Remberg assets API
  slug: remberg-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-assets-api-openapi.yml
- filename: remberg-contacts-api-openapi.yml
  format: yaml
  label: Remberg contacts API
  slug: remberg-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-contacts-api-openapi.yml
- filename: remberg-failure-types-api-openapi.yml
  format: yaml
  label: Remberg failure-types API
  slug: remberg-failure-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-failure-types-api-openapi.yml
- filename: remberg-files-api-openapi.yml
  format: yaml
  label: Remberg files API
  slug: remberg-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-files-api-openapi.yml
- filename: remberg-forms-api-openapi.yml
  format: yaml
  label: Remberg forms API
  slug: remberg-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-forms-api-openapi.yml
- filename: remberg-inventories-api-openapi.yml
  format: yaml
  label: Remberg inventories API
  slug: remberg-inventories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-inventories-api-openapi.yml
- filename: remberg-organizations-api-openapi.yml
  format: yaml
  label: Remberg organizations API
  slug: remberg-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-organizations-api-openapi.yml
- filename: remberg-part-stock-changes-api-openapi.yml
  format: yaml
  label: Remberg part-stock-changes API
  slug: remberg-part-stock-changes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-part-stock-changes-api-openapi.yml
- filename: remberg-parts-api-openapi.yml
  format: yaml
  label: Remberg parts API
  slug: remberg-parts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-parts-api-openapi.yml
- filename: remberg-procedure-templates-api-openapi.yml
  format: yaml
  label: Remberg procedure-templates API
  slug: remberg-procedure-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-procedure-templates-api-openapi.yml
- filename: remberg-tickets-api-openapi.yml
  format: yaml
  label: Remberg tickets API
  slug: remberg-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-tickets-api-openapi.yml
- filename: remberg-user-groups-api-openapi.yml
  format: yaml
  label: Remberg user-groups API
  slug: remberg-user-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-user-groups-api-openapi.yml
- filename: remberg-user-roles-api-openapi.yml
  format: yaml
  label: Remberg user-roles API
  slug: remberg-user-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-user-roles-api-openapi.yml
- filename: remberg-users-api-openapi.yml
  format: yaml
  label: Remberg users API
  slug: remberg-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-users-api-openapi.yml
- filename: remberg-work-orders-api-openapi.yml
  format: yaml
  label: Remberg work-orders API
  slug: remberg-work-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-work-orders-api-openapi.yml
- filename: remberg-work-requests-api-openapi.yml
  format: yaml
  label: Remberg work-requests API
  slug: remberg-work-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-work-requests-api-openapi.yml
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
