---
api_key_in: []
api_specs:
- filename: tango-accounts-api-openapi.yml
  format: yaml
  label: Tango Accounts API
  slug: tango-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango/refs/heads/main/openapi/tango-accounts-api-openapi.yml
- filename: tango-catalog-api-openapi.yml
  format: yaml
  label: Tango Catalog API
  slug: tango-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango/refs/heads/main/openapi/tango-catalog-api-openapi.yml
- filename: tango-customers-api-openapi.yml
  format: yaml
  label: Tango Customers API
  slug: tango-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango/refs/heads/main/openapi/tango-customers-api-openapi.yml
- filename: tango-digital-templates-api-openapi.yml
  format: yaml
  label: Tango Digital Templates API
  slug: tango-digital-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango/refs/heads/main/openapi/tango-digital-templates-api-openapi.yml
- filename: tango-funding-api-openapi.yml
  format: yaml
  label: Tango Funding API
  slug: tango-funding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango/refs/heads/main/openapi/tango-funding-api-openapi.yml
- filename: tango-line-items-api-openapi.yml
  format: yaml
  label: Tango Line Items API
  slug: tango-line-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango/refs/heads/main/openapi/tango-line-items-api-openapi.yml
- filename: tango-low-balance-alerts-api-openapi.yml
  format: yaml
  label: Tango Low Balance Alerts API
  slug: tango-low-balance-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango/refs/heads/main/openapi/tango-low-balance-alerts-api-openapi.yml
- filename: tango-orders-api-openapi.yml
  format: yaml
  label: Tango Orders API
  slug: tango-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango/refs/heads/main/openapi/tango-orders-api-openapi.yml
- filename: tango-reference-data-api-openapi.yml
  format: yaml
  label: Tango Reference Data API
  slug: tango-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango/refs/heads/main/openapi/tango-reference-data-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tango Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tango secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tango
provider_slug: tango
scheme_count: 1
schemes:
- description: HTTP Basic Auth using platform credentials (username/password)
  name: basicAuth
  scheme: basic
  sources:
  - openapi/tango-raas-api-openapi.yml
  type: http
slug: tango-authentication
source_filename: tango-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tango-raas-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Auth using platform credentials (username/password)\n  sources:\n  - openapi/tango-raas-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tango/refs/heads/main/authentication/tango-authentication.yml
summary_line: http · 1 scheme
tags:
- Catalog Management
- Digital Rewards
- Gift Cards
- Incentives
- Loyalty
- Rewards As A Service
---
