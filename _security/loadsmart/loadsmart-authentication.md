---
api_key_in: []
api_specs:
- filename: loadsmart-shipperguide-openapi.yml
  format: yaml
  label: Loadsmart ShipperGuide API
  slug: loadsmart-shipperguide-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loadsmart/refs/heads/main/openapi/loadsmart-shipperguide-openapi.yml
- filename: loadsmart-opendock-openapi.yml
  format: yaml
  label: Opendock Nova (Neutron) API
  slug: loadsmart-opendock-nova-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loadsmart/refs/heads/main/openapi/loadsmart-opendock-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Loadsmart Authentication
name_suffix: Authentication
oauth_flows: []
overview: Loadsmart secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Loadsmart
provider_slug: loadsmart
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearer
  scheme: bearer
  sources:
  - openapi/loadsmart-opendock-openapi.yml
  - openapi/loadsmart-shipperguide-openapi.yml
  type: http
slug: loadsmart-authentication
source_filename: loadsmart-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/loadsmart-opendock-openapi.yml, openapi/loadsmart-shipperguide-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/loadsmart-opendock-openapi.yml\n  - openapi/loadsmart-shipperguide-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loadsmart/refs/heads/main/authentication/loadsmart-authentication.yml
summary_line: http · 1 scheme
tags:
- Freight
- Logistics
- Transportation
- Supply Chain
- Digital Freight
- Freight Brokerage
- Truckload
- LTL
- Drayage
- Flatbed
- Multimodal
- TMS
- Dock Scheduling
- Yard Management
- Warehouse
- 4PL
- FreightTech
---
