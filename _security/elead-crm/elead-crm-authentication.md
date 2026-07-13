---
api_key_in:
- header
api_specs:
- filename: elead-crm-openapi.yml
  format: yaml
  label: Elead Sales Opportunities API
  slug: elead-crm-sales-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elead-crm/refs/heads/main/openapi/elead-crm-openapi.yml
- filename: elead-crm-openapi.yml
  format: yaml
  label: Elead Sales Customers API
  slug: elead-crm-sales-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elead-crm/refs/heads/main/openapi/elead-crm-openapi.yml
- filename: elead-crm-openapi.yml
  format: yaml
  label: Elead Sales Activities API
  slug: elead-crm-sales-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elead-crm/refs/heads/main/openapi/elead-crm-openapi.yml
- filename: elead-crm-openapi.yml
  format: yaml
  label: Elead Product Reference Data API
  slug: elead-crm-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elead-crm/refs/heads/main/openapi/elead-crm-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Elead Crm Authentication
name_suffix: Authentication
oauth_flows: []
overview: Elead secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Elead
provider_slug: elead-crm
scheme_count: 3
schemes:
- description: Fortellis-issued client id for the solution.
  in: header
  name: fortellisClientId
  parameter: client_id
  sources:
  - openapi/elead-crm-openapi.yml
  type: apiKey
- description: Fortellis-issued client secret for the solution.
  in: header
  name: fortellisClientSecret
  parameter: client_secret
  sources:
  - openapi/elead-crm-openapi.yml
  type: apiKey
- description: Per-dealer subscription identifier provided when the dealer activates the app.
  in: header
  name: subscriptionId
  parameter: Subscription-Id
  sources:
  - openapi/elead-crm-openapi.yml
  type: apiKey
slug: elead-crm-authentication
source_filename: elead-crm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/elead-crm-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: fortellisClientId\n  type: apiKey\n  in: header\n  parameter: client_id\n  description: Fortellis-issued client id for the solution.\n  sources:\n  - openapi/elead-crm-openapi.yml\n- name: fortellisClientSecret\n  type: apiKey\n  in: header\n  parameter: client_secret\n  description: Fortellis-issued client secret for the solution.\n  sources:\n  - openapi/elead-crm-openapi.yml\n- name: subscriptionId\n  type: apiKey\n  in: header\n  parameter: Subscription-Id\n  description: Per-dealer subscription identifier provided when the dealer activates the app.\n  sources:\n  - openapi/elead-crm-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elead-crm/refs/heads/main/authentication/elead-crm-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- CRM
- Automotive
- Dealership
- Sales
- Leads
- Fortellis
- CDK Global
---
