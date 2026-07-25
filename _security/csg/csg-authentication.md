---
api_key_in: []
api_specs:
- filename: csg-customers-api-openapi.yml
  format: yaml
  label: CSG Systems Customers API
  slug: csg-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/csg/refs/heads/main/openapi/csg-customers-api-openapi.yml
- filename: csg-payment-methods-api-openapi.yml
  format: yaml
  label: CSG Systems Payment Methods API
  slug: csg-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/csg/refs/heads/main/openapi/csg-payment-methods-api-openapi.yml
- filename: csg-settlements-api-openapi.yml
  format: yaml
  label: CSG Systems Settlements API
  slug: csg-settlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/csg/refs/heads/main/openapi/csg-settlements-api-openapi.yml
- filename: csg-transactions-api-openapi.yml
  format: yaml
  label: CSG Systems Transactions API
  slug: csg-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/csg/refs/heads/main/openapi/csg-transactions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Csg Authentication
name_suffix: Authentication
oauth_flows: []
overview: CSG Systems secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CSG Systems
provider_slug: csg
scheme_count: 1
schemes:
- description: HTTP Basic authentication using API access ID as username and API secure key as password. Include organization ID and location ID in the X-Forte-Auth-Organization-Id and X-Forte-Auth-Location-Id request headers.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/csg-forte-rest-openapi.yml
  type: http
slug: csg-authentication
source_filename: csg-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/csg-forte-rest-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using API access ID as username and API secure key\n    as password. Include organization ID and location ID in the X-Forte-Auth-Organization-Id\n    and X-Forte-Auth-Location-Id request headers.\n  sources:\n  - openapi/csg-forte-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/csg/refs/heads/main/authentication/csg-authentication.yml
summary_line: http · 1 scheme
tags:
- Billing
- Customer Engagement
- Payments
- Revenue Management
- Telecom
---
