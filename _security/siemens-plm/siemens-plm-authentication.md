---
api_key_in:
- header
api_specs:
- filename: tcpcm-api-spec.yaml
  format: yaml
  label: Teamcenter Product Cost Management REST API
  slug: teamcenter-product-cost-management
  spec_type: OpenAPI
  url: https://developer.siemens.com/tcpcm/tcpcm-api-spec.yaml
- filename: polarion-rest-apispec.json
  format: json
  label: Polarion REST API
  slug: polarion-rest-api
  spec_type: OpenAPI
  url: https://developer.siemens.com/polarion/polarion-rest-apispec.json
- filename: product-information-api.spec.yaml
  format: yaml
  label: Product Information API
  slug: product-information-api
  spec_type: OpenAPI
  url: https://developer.siemens.com/product-information-api/product-information-api.spec.yaml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Siemens Plm Authentication
name_suffix: Authentication
oauth_flows: []
overview: Siemens PLM secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Siemens PLM
provider_slug: siemens-plm
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/polarion-rest-api.json
  - openapi/teamcenter-product-cost-management.yaml
  type: http
- in: header
  name: Authorization
  parameter: Authorization
  sources:
  - openapi/product-information-api.yaml
  type: apiKey
slug: siemens-plm-authentication
source_filename: siemens-plm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/polarion-rest-api.json, openapi/product-information-api.yaml, openapi/teamcenter-product-cost-management.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/polarion-rest-api.json\n  - openapi/teamcenter-product-cost-management.yaml\n- name: Authorization\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/product-information-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/siemens-plm/refs/heads/main/authentication/siemens-plm-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- PLM
- Product Lifecycle Management
- Teamcenter
- NX
- Solid Edge
- Simcenter
- Xcelerator
- Digital Manufacturing
- Industrial IoT
- CAD
- CAM
- Sustainability
- ALM
---
