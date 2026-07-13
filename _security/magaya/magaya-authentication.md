---
api_key_in: []
api_specs:
- filename: magaya-openapi.yml
  format: yaml
  label: Magaya Shipments API
  slug: magaya-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magaya/refs/heads/main/openapi/magaya-openapi.yml
- filename: magaya-openapi.yml
  format: yaml
  label: Magaya Warehouse Receipts API
  slug: magaya-warehouse-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magaya/refs/heads/main/openapi/magaya-openapi.yml
- filename: magaya-openapi.yml
  format: yaml
  label: Magaya Invoices API
  slug: magaya-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magaya/refs/heads/main/openapi/magaya-openapi.yml
- filename: magaya-openapi.yml
  format: yaml
  label: Magaya Items API
  slug: magaya-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magaya/refs/heads/main/openapi/magaya-openapi.yml
- filename: magaya-openapi.yml
  format: yaml
  label: Magaya Transactions API
  slug: magaya-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magaya/refs/heads/main/openapi/magaya-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Magaya Authentication
name_suffix: Authentication
oauth_flows: []
overview: Magaya secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Magaya
provider_slug: magaya
scheme_count: 1
schemes:
- description: Magaya API user. A dedicated API user (username and password) is configured inside the Magaya system, distinct from a regular login user. The Digital Freight Portal REST API instead uses Auth0 machine-to-machine OAuth client credentials.
  name: apiUser
  scheme: basic
  sources:
  - openapi/magaya-openapi.yml
  type: http
slug: magaya-authentication
source_filename: magaya-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/magaya-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiUser\n  type: http\n  scheme: basic\n  description: Magaya API user. A dedicated API user (username and password) is configured inside\n    the Magaya system, distinct from a regular login user. The Digital Freight Portal REST API\n    instead uses Auth0 machine-to-machine OAuth client credentials.\n  sources:\n  - openapi/magaya-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/magaya/refs/heads/main/authentication/magaya-authentication.yml
summary_line: http · 1 scheme
tags:
- Logistics
- Supply Chain
- Freight Forwarding
- Warehouse Management
- Shipping
- Customs
- Transportation
---
