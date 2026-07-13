---
api_key_in:
- header
api_specs:
- filename: locus-oms-openapi.yml
  format: yaml
  label: Locus Order Management API
  slug: locus-order-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-oms-openapi.yml
- filename: locus-entities-openapi.yml
  format: yaml
  label: Locus Entity Management API
  slug: locus-entity-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-entities-openapi.yml
- filename: locus-platform-openapi.yml
  format: yaml
  label: Locus Platform Entities API
  slug: locus-platform-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-platform-openapi.yml
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
