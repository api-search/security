---
api_key_in: []
api_specs:
- filename: tech-data-authentication-api-openapi.yml
  format: yaml
  label: Tech Data Authentication API
  slug: tech-data-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tech-data/refs/heads/main/openapi/tech-data-authentication-api-openapi.yml
- filename: tech-data-cart-items-api-openapi.yml
  format: yaml
  label: Tech Data Cart Items API
  slug: tech-data-cart-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tech-data/refs/heads/main/openapi/tech-data-cart-items-api-openapi.yml
- filename: tech-data-carts-api-openapi.yml
  format: yaml
  label: Tech Data Carts API
  slug: tech-data-carts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tech-data/refs/heads/main/openapi/tech-data-carts-api-openapi.yml
- filename: tech-data-cloud-providers-api-openapi.yml
  format: yaml
  label: Tech Data Cloud Providers API
  slug: tech-data-cloud-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tech-data/refs/heads/main/openapi/tech-data-cloud-providers-api-openapi.yml
- filename: tech-data-customers-api-openapi.yml
  format: yaml
  label: Tech Data Customers API
  slug: tech-data-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tech-data/refs/heads/main/openapi/tech-data-customers-api-openapi.yml
- filename: tech-data-orders-api-openapi.yml
  format: yaml
  label: Tech Data Orders API
  slug: tech-data-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tech-data/refs/heads/main/openapi/tech-data-orders-api-openapi.yml
- filename: tech-data-products-api-openapi.yml
  format: yaml
  label: Tech Data Products API
  slug: tech-data-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tech-data/refs/heads/main/openapi/tech-data-products-api-openapi.yml
- filename: tech-data-provisioning-templates-api-openapi.yml
  format: yaml
  label: Tech Data Provisioning Templates API
  slug: tech-data-provisioning-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tech-data/refs/heads/main/openapi/tech-data-provisioning-templates-api-openapi.yml
- filename: tech-data-reports-api-openapi.yml
  format: yaml
  label: Tech Data Reports API
  slug: tech-data-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tech-data/refs/heads/main/openapi/tech-data-reports-api-openapi.yml
- filename: tech-data-subscriptions-api-openapi.yml
  format: yaml
  label: Tech Data Subscriptions API
  slug: tech-data-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tech-data/refs/heads/main/openapi/tech-data-subscriptions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tech Data Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tech Data secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tech Data
provider_slug: tech-data
scheme_count: 1
schemes:
- description: OAuth 2.0 bearer token obtained via the /oauth/token endpoint.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/streamone-ion-openapi.yml
  type: http
slug: tech-data-authentication
source_filename: tech-data-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/streamone-ion-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 bearer token obtained via the /oauth/token endpoint.\n  sources:\n  - openapi/streamone-ion-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tech-data/refs/heads/main/authentication/tech-data-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud
- Distribution
- Information Technology
- Partner
- Fortune 500
---
