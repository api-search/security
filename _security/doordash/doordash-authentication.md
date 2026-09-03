---
api_key_in: []
api_specs:
- filename: doordash-addresses-api-openapi.yml
  format: yaml
  label: doordash Addresses API
  slug: doordash-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-addresses-api-openapi.yml
- filename: doordash-businesses-api-openapi.yml
  format: yaml
  label: doordash Businesses API
  slug: doordash-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-businesses-api-openapi.yml
- filename: doordash-catalog-api-openapi.yml
  format: yaml
  label: doordash Catalog API
  slug: doordash-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-catalog-api-openapi.yml
- filename: doordash-deliveries-api-openapi.yml
  format: yaml
  label: doordash Deliveries API
  slug: doordash-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-deliveries-api-openapi.yml
- filename: doordash-inventory-api-openapi.yml
  format: yaml
  label: doordash Inventory API
  slug: doordash-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-inventory-api-openapi.yml
- filename: doordash-items-api-openapi.yml
  format: yaml
  label: doordash Items API
  slug: doordash-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-items-api-openapi.yml
- filename: doordash-menus-api-openapi.yml
  format: yaml
  label: doordash Menus API
  slug: doordash-menus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-menus-api-openapi.yml
- filename: doordash-orders-api-openapi.yml
  format: yaml
  label: doordash Orders API
  slug: doordash-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-orders-api-openapi.yml
- filename: doordash-promotions-api-openapi.yml
  format: yaml
  label: doordash Promotions API
  slug: doordash-promotions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-promotions-api-openapi.yml
- filename: doordash-quotes-api-openapi.yml
  format: yaml
  label: doordash Quotes API
  slug: doordash-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-quotes-api-openapi.yml
- filename: doordash-reports-api-openapi.yml
  format: yaml
  label: doordash Reports API
  slug: doordash-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-reports-api-openapi.yml
- filename: doordash-stores-api-openapi.yml
  format: yaml
  label: doordash Stores API
  slug: doordash-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-stores-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Doordash Authentication
name_suffix: Authentication
oauth_flows: []
overview: Doordash secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Doordash
provider_slug: doordash
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT token signed with your DoorDash developer credentials.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/doordash-drive-classic-openapi.yml
  - openapi/doordash-drive-openapi.yml
  - openapi/doordash-item-management-openapi.yml
  - openapi/doordash-marketplace-openapi.yml
  - openapi/doordash-reporting-openapi.yml
  type: http
slug: doordash-authentication
source_filename: doordash-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/doordash-drive-classic-openapi.yml, openapi/doordash-drive-openapi.yml, openapi/doordash-item-management-openapi.yml,\n  openapi/doordash-marketplace-openapi.yml, openapi/doordash-reporting-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token signed with your DoorDash developer credentials.\n  sources:\n  - openapi/doordash-drive-classic-openapi.yml\n  - openapi/doordash-drive-openapi.yml\n  - openapi/doordash-item-management-openapi.yml\n  - openapi/doordash-marketplace-openapi.yml\n  - openapi/doordash-reporting-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/authentication/doordash-authentication.yml
summary_line: http · 1 scheme
tags: []
---
