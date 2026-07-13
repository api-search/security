---
api_key_in:
- header
api_specs:
- filename: shipwell-openapi.yml
  format: yaml
  label: Shipwell Shipments API
  slug: shipwell-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipwell/refs/heads/main/openapi/shipwell-openapi.yml
- filename: shipwell-openapi.yml
  format: yaml
  label: Shipwell Quoting and Rating API
  slug: shipwell-quoting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipwell/refs/heads/main/openapi/shipwell-openapi.yml
- filename: shipwell-openapi.yml
  format: yaml
  label: Shipwell Carriers API
  slug: shipwell-carriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipwell/refs/heads/main/openapi/shipwell-openapi.yml
- filename: shipwell-openapi.yml
  format: yaml
  label: Shipwell Orders API
  slug: shipwell-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipwell/refs/heads/main/openapi/shipwell-openapi.yml
- filename: shipwell-openapi.yml
  format: yaml
  label: Shipwell Events and Webhooks API
  slug: shipwell-events-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipwell/refs/heads/main/openapi/shipwell-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Shipwell Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shipwell secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Shipwell
provider_slug: shipwell
scheme_count: 1
schemes:
- description: Company-scoped API key passed in the Authorization header (the docs refer to this as the AuthToken scheme). Production and sandbox use separate keys. Keys can be permission-restricted.
  in: header
  name: authToken
  parameter: Authorization
  sources:
  - openapi/shipwell-openapi.yml
  type: apiKey
slug: shipwell-authentication
source_filename: shipwell-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shipwell-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: authToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Company-scoped API key passed in the Authorization header (the docs refer to\n    this as the AuthToken scheme). Production and sandbox use separate keys. Keys can be permission-restricted.\n  sources:\n  - openapi/shipwell-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shipwell/refs/heads/main/authentication/shipwell-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Transportation Management
- TMS
- Freight
- Logistics
- Shipping
- Supply Chain
---
