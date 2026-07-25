---
api_key_in:
- header
api_specs:
- filename: upkeep-assets-api-openapi.yml
  format: yaml
  label: UpKeep Assets API
  slug: upkeep-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upkeep/refs/heads/main/openapi/upkeep-assets-api-openapi.yml
- filename: upkeep-authentication-api-openapi.yml
  format: yaml
  label: UpKeep Authentication API
  slug: upkeep-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upkeep/refs/heads/main/openapi/upkeep-authentication-api-openapi.yml
- filename: upkeep-locations-api-openapi.yml
  format: yaml
  label: UpKeep Locations API
  slug: upkeep-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upkeep/refs/heads/main/openapi/upkeep-locations-api-openapi.yml
- filename: upkeep-meters-api-openapi.yml
  format: yaml
  label: UpKeep Meters API
  slug: upkeep-meters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upkeep/refs/heads/main/openapi/upkeep-meters-api-openapi.yml
- filename: upkeep-parts-api-openapi.yml
  format: yaml
  label: UpKeep Parts API
  slug: upkeep-parts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upkeep/refs/heads/main/openapi/upkeep-parts-api-openapi.yml
- filename: upkeep-preventive-maintenance-api-openapi.yml
  format: yaml
  label: UpKeep Preventive Maintenance API
  slug: upkeep-preventive-maintenance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upkeep/refs/heads/main/openapi/upkeep-preventive-maintenance-api-openapi.yml
- filename: upkeep-purchase-orders-api-openapi.yml
  format: yaml
  label: UpKeep Purchase Orders API
  slug: upkeep-purchase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upkeep/refs/heads/main/openapi/upkeep-purchase-orders-api-openapi.yml
- filename: upkeep-requests-api-openapi.yml
  format: yaml
  label: UpKeep Requests API
  slug: upkeep-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upkeep/refs/heads/main/openapi/upkeep-requests-api-openapi.yml
- filename: upkeep-webhooks-api-openapi.yml
  format: yaml
  label: UpKeep Webhooks API
  slug: upkeep-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upkeep/refs/heads/main/openapi/upkeep-webhooks-api-openapi.yml
- filename: upkeep-work-orders-api-openapi.yml
  format: yaml
  label: UpKeep Work Orders API
  slug: upkeep-work-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upkeep/refs/heads/main/openapi/upkeep-work-orders-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Upkeep Authentication
name_suffix: Authentication
oauth_flows: []
overview: UpKeep secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: UpKeep
provider_slug: upkeep
scheme_count: 1
schemes:
- description: Session token obtained from POST /auth
  in: header
  name: SessionToken
  parameter: session-token
  sources:
  - openapi/upkeep-openapi.yml
  type: apiKey
slug: upkeep-authentication
source_filename: upkeep-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/upkeep-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SessionToken\n  type: apiKey\n  in: header\n  parameter: session-token\n  description: Session token obtained from POST /auth\n  sources:\n  - openapi/upkeep-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upkeep/refs/heads/main/authentication/upkeep-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- CMMS
- Maintenance Management
- Asset Management
- Facility Management
- Work Orders
---
