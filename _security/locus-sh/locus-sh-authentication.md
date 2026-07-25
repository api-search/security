---
api_key_in:
- header
api_specs:
- filename: locus-sh-homebasemaster-api-openapi.yml
  format: yaml
  label: Locus HomebaseMaster API
  slug: locus-sh-homebasemaster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-sh-homebasemaster-api-openapi.yml
- filename: locus-sh-locationmaster-api-openapi.yml
  format: yaml
  label: Locus LocationMaster API
  slug: locus-sh-locationmaster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-sh-locationmaster-api-openapi.yml
- filename: locus-sh-order-api-openapi.yml
  format: yaml
  label: Locus Order API
  slug: locus-sh-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-sh-order-api-openapi.yml
- filename: locus-sh-orderserviceability-api-openapi.yml
  format: yaml
  label: Locus OrderServiceability API
  slug: locus-sh-orderserviceability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-sh-orderserviceability-api-openapi.yml
- filename: locus-sh-personnelmaster-api-openapi.yml
  format: yaml
  label: Locus PersonnelMaster API
  slug: locus-sh-personnelmaster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-sh-personnelmaster-api-openapi.yml
- filename: locus-sh-rider-api-openapi.yml
  format: yaml
  label: Locus Rider API
  slug: locus-sh-rider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-sh-rider-api-openapi.yml
- filename: locus-sh-riderpersona-api-openapi.yml
  format: yaml
  label: Locus RiderPersona API
  slug: locus-sh-riderpersona-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-sh-riderpersona-api-openapi.yml
- filename: locus-sh-roster-api-openapi.yml
  format: yaml
  label: Locus Roster API
  slug: locus-sh-roster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-sh-roster-api-openapi.yml
- filename: locus-sh-servicetype-api-openapi.yml
  format: yaml
  label: Locus ServiceType API
  slug: locus-sh-servicetype-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-sh-servicetype-api-openapi.yml
- filename: locus-sh-servicetypeconfiguration-api-openapi.yml
  format: yaml
  label: Locus ServiceTypeConfiguration API
  slug: locus-sh-servicetypeconfiguration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-sh-servicetypeconfiguration-api-openapi.yml
- filename: locus-sh-shifttag-api-openapi.yml
  format: yaml
  label: Locus ShiftTag API
  slug: locus-sh-shifttag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-sh-shifttag-api-openapi.yml
- filename: locus-sh-skumaster-api-openapi.yml
  format: yaml
  label: Locus SKUMaster API
  slug: locus-sh-skumaster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-sh-skumaster-api-openapi.yml
- filename: locus-sh-teammaster-api-openapi.yml
  format: yaml
  label: Locus TeamMaster API
  slug: locus-sh-teammaster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-sh-teammaster-api-openapi.yml
- filename: locus-sh-transporter-api-openapi.yml
  format: yaml
  label: Locus Transporter API
  slug: locus-sh-transporter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-sh-transporter-api-openapi.yml
- filename: locus-sh-vehicle-api-openapi.yml
  format: yaml
  label: Locus Vehicle API
  slug: locus-sh-vehicle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-sh-vehicle-api-openapi.yml
- filename: locus-sh-vehiclemodel-api-openapi.yml
  format: yaml
  label: Locus VehicleModel API
  slug: locus-sh-vehiclemodel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-sh-vehiclemodel-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Locus Sh Authentication
name_suffix: Authentication
oauth_flows: []
overview: Locus secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Locus
provider_slug: locus-sh
scheme_count: 2
schemes:
- description: HTTP Basic Authentication
  name: locusauth
  scheme: basic
  sources:
  - openapi/locus-entities-openapi.yml
  - openapi/locus-oms-openapi.yml
  - openapi/locus-platform-openapi.yml
  type: http
- in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/locus-entities-openapi.yml
  - openapi/locus-oms-openapi.yml
  - openapi/locus-platform-openapi.yml
  type: apiKey
slug: locus-sh-authentication
source_filename: locus-sh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/locus-entities-openapi.yml, openapi/locus-oms-openapi.yml, openapi/locus-platform-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: locusauth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication\n  sources:\n  - openapi/locus-entities-openapi.yml\n  - openapi/locus-oms-openapi.yml\n  - openapi/locus-platform-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/locus-entities-openapi.yml\n  - openapi/locus-oms-openapi.yml\n  - openapi/locus-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/authentication/locus-sh-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Logistics
- Last Mile Delivery
- Route Optimization
- Dispatch Planning
- Transportation Management
- Fleet Management
- Supply Chain
- Order Management
- Fulfillment
- Track and Trace
- Retail
- E-Commerce
- Artificial Intelligence
- India
---
