---
api_key_in:
- header
api_specs:
- filename: zuper-assets-api-openapi.yml
  format: yaml
  label: Zuper Assets API
  slug: zuper-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuper/refs/heads/main/openapi/zuper-assets-api-openapi.yml
- filename: zuper-authentication-api-openapi.yml
  format: yaml
  label: Zuper Authentication API
  slug: zuper-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuper/refs/heads/main/openapi/zuper-authentication-api-openapi.yml
- filename: zuper-customers-api-openapi.yml
  format: yaml
  label: Zuper Customers API
  slug: zuper-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuper/refs/heads/main/openapi/zuper-customers-api-openapi.yml
- filename: zuper-invoices-api-openapi.yml
  format: yaml
  label: Zuper Invoices API
  slug: zuper-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuper/refs/heads/main/openapi/zuper-invoices-api-openapi.yml
- filename: zuper-jobs-api-openapi.yml
  format: yaml
  label: Zuper Jobs API
  slug: zuper-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuper/refs/heads/main/openapi/zuper-jobs-api-openapi.yml
- filename: zuper-organizations-api-openapi.yml
  format: yaml
  label: Zuper Organizations API
  slug: zuper-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuper/refs/heads/main/openapi/zuper-organizations-api-openapi.yml
- filename: zuper-projects-api-openapi.yml
  format: yaml
  label: Zuper Projects API
  slug: zuper-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuper/refs/heads/main/openapi/zuper-projects-api-openapi.yml
- filename: zuper-properties-api-openapi.yml
  format: yaml
  label: Zuper Properties API
  slug: zuper-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuper/refs/heads/main/openapi/zuper-properties-api-openapi.yml
- filename: zuper-purchase-orders-api-openapi.yml
  format: yaml
  label: Zuper Purchase Orders API
  slug: zuper-purchase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuper/refs/heads/main/openapi/zuper-purchase-orders-api-openapi.yml
- filename: zuper-teams-api-openapi.yml
  format: yaml
  label: Zuper Teams API
  slug: zuper-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuper/refs/heads/main/openapi/zuper-teams-api-openapi.yml
- filename: zuper-timesheets-api-openapi.yml
  format: yaml
  label: Zuper Timesheets API
  slug: zuper-timesheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuper/refs/heads/main/openapi/zuper-timesheets-api-openapi.yml
- filename: zuper-users-api-openapi.yml
  format: yaml
  label: Zuper Users API
  slug: zuper-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuper/refs/heads/main/openapi/zuper-users-api-openapi.yml
- filename: zuper-vendors-api-openapi.yml
  format: yaml
  label: Zuper Vendors API
  slug: zuper-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuper/refs/heads/main/openapi/zuper-vendors-api-openapi.yml
- filename: zuper-webhooks-api-openapi.yml
  format: yaml
  label: Zuper Webhooks API
  slug: zuper-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuper/refs/heads/main/openapi/zuper-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Zuper Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zuper secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zuper
provider_slug: zuper
scheme_count: 1
schemes:
- description: API key generated from Zuper Settings > Developer Hub > API Keys
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/zuper-rest-api-openapi.yml
  type: apiKey
slug: zuper-authentication
source_filename: zuper-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zuper-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key generated from Zuper Settings > Developer Hub > API Keys\n  sources:\n  - openapi/zuper-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zuper/refs/heads/main/authentication/zuper-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Field Service Management
- Scheduling
- Dispatching
- Invoicing
- Timesheets
- Asset Management
- Work Orders
- Customer Management
- Inventory
- Projects
---
