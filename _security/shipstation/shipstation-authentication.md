---
api_key_in: []
api_specs:
- filename: shipstation-v1-openapi.yml
  format: yaml
  label: ShipStation V1 API
  slug: shipstation-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipstation/refs/heads/main/openapi/shipstation-v1-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Shipstation Authentication
name_suffix: Authentication
oauth_flows: []
overview: ShipStation secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ShipStation
provider_slug: shipstation
scheme_count: 1
schemes:
- description: HTTP Basic authentication using API Key as username and API Secret as password
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/shipstation-v1-openapi.yml
  type: http
slug: shipstation-authentication
source_filename: shipstation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shipstation-v1-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using API Key as username and API Secret as password\n  sources:\n  - openapi/shipstation-v1-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shipstation/refs/heads/main/authentication/shipstation-authentication.yml
summary_line: http · 1 scheme
tags:
- Ecommerce
- Labels
- Logistics
- Order Management
- Shipping
- Warehousing
---
