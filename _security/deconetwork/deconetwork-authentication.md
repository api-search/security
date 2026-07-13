---
api_key_in:
- query
api_specs:
- filename: deconetwork-openapi.yml
  format: yaml
  label: DecoNetwork Order Management API
  slug: deconetwork-order-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deconetwork/refs/heads/main/openapi/deconetwork-openapi.yml
- filename: deconetwork-openapi.yml
  format: yaml
  label: DecoNetwork Product Management API
  slug: deconetwork-product-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deconetwork/refs/heads/main/openapi/deconetwork-openapi.yml
- filename: deconetwork-openapi.yml
  format: yaml
  label: DecoNetwork Inventory Management API
  slug: deconetwork-inventory-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deconetwork/refs/heads/main/openapi/deconetwork-openapi.yml
- filename: deconetwork-openapi.yml
  format: yaml
  label: DecoNetwork Purchase Order Management API
  slug: deconetwork-purchase-order-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deconetwork/refs/heads/main/openapi/deconetwork-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Deconetwork Authentication
name_suffix: Authentication
oauth_flows: []
overview: DecoNetwork secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DecoNetwork
provider_slug: deconetwork
scheme_count: 1
schemes:
- description: DecoNetwork authenticates each request with username and password fields passed as query parameters (GET/POST) or in the form-encoded body. Both fields are required on every request.
  in: query
  name: credentials
  parameter: username
  sources:
  - openapi/deconetwork-openapi.yml
  type: apiKey
slug: deconetwork-authentication
source_filename: deconetwork-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/deconetwork-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: credentials\n  type: apiKey\n  in: query\n  parameter: username\n  description: DecoNetwork authenticates each request with username and password fields passed\n    as query parameters (GET/POST) or in the form-encoded body. Both fields are required on\n    every request.\n  sources:\n  - openapi/deconetwork-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deconetwork/refs/heads/main/authentication/deconetwork-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Custom Apparel
- Web to Print
- Print Shop Management
- Orders
- Products
- Inventory
- Production Workflow
- E-commerce
---
