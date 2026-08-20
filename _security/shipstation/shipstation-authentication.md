---
api_key_in: []
api_specs:
- filename: shipstation-accounts-api-openapi.yml
  format: yaml
  label: ShipStation Accounts API
  slug: shipstation-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipstation/refs/heads/main/openapi/shipstation-accounts-api-openapi.yml
- filename: shipstation-carriers-api-openapi.yml
  format: yaml
  label: ShipStation Carriers API
  slug: shipstation-carriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipstation/refs/heads/main/openapi/shipstation-carriers-api-openapi.yml
- filename: shipstation-customers-api-openapi.yml
  format: yaml
  label: ShipStation Customers API
  slug: shipstation-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipstation/refs/heads/main/openapi/shipstation-customers-api-openapi.yml
- filename: shipstation-fulfillments-api-openapi.yml
  format: yaml
  label: ShipStation Fulfillments API
  slug: shipstation-fulfillments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipstation/refs/heads/main/openapi/shipstation-fulfillments-api-openapi.yml
- filename: shipstation-orders-api-openapi.yml
  format: yaml
  label: ShipStation Orders API
  slug: shipstation-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipstation/refs/heads/main/openapi/shipstation-orders-api-openapi.yml
- filename: shipstation-products-api-openapi.yml
  format: yaml
  label: ShipStation Products API
  slug: shipstation-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipstation/refs/heads/main/openapi/shipstation-products-api-openapi.yml
- filename: shipstation-shipments-api-openapi.yml
  format: yaml
  label: ShipStation Shipments API
  slug: shipstation-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipstation/refs/heads/main/openapi/shipstation-shipments-api-openapi.yml
- filename: shipstation-stores-api-openapi.yml
  format: yaml
  label: ShipStation Stores API
  slug: shipstation-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipstation/refs/heads/main/openapi/shipstation-stores-api-openapi.yml
- filename: shipstation-warehouses-api-openapi.yml
  format: yaml
  label: ShipStation Warehouses API
  slug: shipstation-warehouses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipstation/refs/heads/main/openapi/shipstation-warehouses-api-openapi.yml
- filename: shipstation-webhooks-api-openapi.yml
  format: yaml
  label: ShipStation Webhooks API
  slug: shipstation-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipstation/refs/heads/main/openapi/shipstation-webhooks-api-openapi.yml
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
- E-Commerce
- Labels
- Logistics
- Order Management
- Shipping
- Warehousing
---
