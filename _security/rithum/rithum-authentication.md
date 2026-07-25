---
api_key_in: []
api_specs:
- filename: rithum-authentication-api-openapi.yml
  format: yaml
  label: Rithum Authentication API
  slug: rithum-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rithum/refs/heads/main/openapi/rithum-authentication-api-openapi.yml
- filename: rithum-catalog-api-openapi.yml
  format: yaml
  label: Rithum Catalog API
  slug: rithum-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rithum/refs/heads/main/openapi/rithum-catalog-api-openapi.yml
- filename: rithum-inventory-api-openapi.yml
  format: yaml
  label: Rithum Inventory API
  slug: rithum-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rithum/refs/heads/main/openapi/rithum-inventory-api-openapi.yml
- filename: rithum-invoices-api-openapi.yml
  format: yaml
  label: Rithum Invoices API
  slug: rithum-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rithum/refs/heads/main/openapi/rithum-invoices-api-openapi.yml
- filename: rithum-orders-api-openapi.yml
  format: yaml
  label: Rithum Orders API
  slug: rithum-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rithum/refs/heads/main/openapi/rithum-orders-api-openapi.yml
- filename: rithum-returns-api-openapi.yml
  format: yaml
  label: Rithum Returns API
  slug: rithum-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rithum/refs/heads/main/openapi/rithum-returns-api-openapi.yml
- filename: rithum-shipments-api-openapi.yml
  format: yaml
  label: Rithum Shipments API
  slug: rithum-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rithum/refs/heads/main/openapi/rithum-shipments-api-openapi.yml
- filename: rithum-streams-api-openapi.yml
  format: yaml
  label: Rithum Streams API
  slug: rithum-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rithum/refs/heads/main/openapi/rithum-streams-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Rithum Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rithum secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rithum
provider_slug: rithum
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/dsco-platform-openapi.yml
  type: http
slug: rithum-authentication
source_filename: rithum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dsco-platform-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/dsco-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rithum/refs/heads/main/authentication/rithum-authentication.yml
summary_line: http · 1 scheme
tags:
- Commerce
- Dropship
- Marketplace
- Ecommerce
- Supply Chain
- Retail
---
