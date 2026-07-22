---
api_key_in:
- header
api_specs:
- filename: scoutrfp-suppliers-v1-openapi.json
  format: json
  label: Workday Strategic Sourcing - Suppliers API
  slug: workday-strategic-sourcing-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/openapi/scoutrfp-suppliers-v1-openapi.json
- filename: scoutrfp-events-v1-openapi.json
  format: json
  label: Workday Strategic Sourcing - Events API
  slug: workday-strategic-sourcing-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/openapi/scoutrfp-events-v1-openapi.json
- filename: scoutrfp-reports-v1-openapi.json
  format: json
  label: Workday Strategic Sourcing - Reports API
  slug: workday-strategic-sourcing-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/openapi/scoutrfp-reports-v1-openapi.json
- filename: scoutrfp-contracts-v1-openapi.json
  format: json
  label: Workday Strategic Sourcing - Contracts API
  slug: workday-strategic-sourcing-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/openapi/scoutrfp-contracts-v1-openapi.json
- filename: scoutrfp-projects-v1-openapi.json
  format: json
  label: Workday Strategic Sourcing - Projects API
  slug: workday-strategic-sourcing-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/openapi/scoutrfp-projects-v1-openapi.json
- filename: scoutrfp-payments-v1-openapi.json
  format: json
  label: Workday Strategic Sourcing - Payments API
  slug: workday-strategic-sourcing-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/openapi/scoutrfp-payments-v1-openapi.json
- filename: scoutrfp-fields-v1-openapi.json
  format: json
  label: Workday Strategic Sourcing - Fields API
  slug: workday-strategic-sourcing-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/openapi/scoutrfp-fields-v1-openapi.json
- filename: scoutrfp-awards-v1-openapi.json
  format: json
  label: Workday Strategic Sourcing - Awards API
  slug: workday-strategic-sourcing-awards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/openapi/scoutrfp-awards-v1-openapi.json
- filename: scoutrfp-attachments-v1-openapi.json
  format: json
  label: Workday Strategic Sourcing - Attachments API
  slug: workday-strategic-sourcing-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/openapi/scoutrfp-attachments-v1-openapi.json
- filename: scoutrfp-spend_categories-v1-openapi.json
  format: json
  label: Workday Strategic Sourcing - Spend Categories API
  slug: workday-strategic-sourcing-spend-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/openapi/scoutrfp-spend_categories-v1-openapi.json
- filename: scoutrfp-scim-v2-openapi.json
  format: json
  label: Workday Strategic Sourcing - SCIM (Users) API
  slug: workday-strategic-sourcing-scim-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/openapi/scoutrfp-scim-v2-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Scoutrfp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scout RFP (Workday Strategic Sourcing) secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Scout RFP (Workday Strategic Sourcing)
provider_slug: scoutrfp
scheme_count: 4
schemes:
- description: Company API key.
  in: header
  name: api_key
  parameter: X-Api-Key
  sources:
  - openapi/scoutrfp-attachments-v1-openapi.json
  - openapi/scoutrfp-awards-v1-openapi.json
  - openapi/scoutrfp-contracts-v1-openapi.json
  - openapi/scoutrfp-events-v1-openapi.json
  - openapi/scoutrfp-fields-v1-openapi.json
  - openapi/scoutrfp-payments-v1-openapi.json
  - openapi/scoutrfp-projects-v1-openapi.json
  - openapi/scoutrfp-reports-v1-openapi.json
  - openapi/scoutrfp-scim-v2-openapi.json
  - openapi/scoutrfp-spend_categories-v1-openapi.json
  - openapi/scoutrfp-suppliers-v1-openapi.json
  type: apiKey
- description: User token.
  in: header
  name: user_token
  parameter: X-User-Token
  sources:
  - openapi/scoutrfp-attachments-v1-openapi.json
  - openapi/scoutrfp-awards-v1-openapi.json
  - openapi/scoutrfp-contracts-v1-openapi.json
  - openapi/scoutrfp-events-v1-openapi.json
  - openapi/scoutrfp-fields-v1-openapi.json
  - openapi/scoutrfp-payments-v1-openapi.json
  - openapi/scoutrfp-projects-v1-openapi.json
  - openapi/scoutrfp-reports-v1-openapi.json
  - openapi/scoutrfp-spend_categories-v1-openapi.json
  - openapi/scoutrfp-suppliers-v1-openapi.json
  type: apiKey
- description: User email.
  in: header
  name: user_email
  parameter: X-User-Email
  sources:
  - openapi/scoutrfp-attachments-v1-openapi.json
  - openapi/scoutrfp-awards-v1-openapi.json
  - openapi/scoutrfp-contracts-v1-openapi.json
  - openapi/scoutrfp-events-v1-openapi.json
  - openapi/scoutrfp-fields-v1-openapi.json
  - openapi/scoutrfp-payments-v1-openapi.json
  - openapi/scoutrfp-projects-v1-openapi.json
  - openapi/scoutrfp-reports-v1-openapi.json
  - openapi/scoutrfp-spend_categories-v1-openapi.json
  - openapi/scoutrfp-suppliers-v1-openapi.json
  type: apiKey
- name: basic_authentication
  scheme: basic
  sources:
  - openapi/scoutrfp-scim-v2-openapi.json
  type: http
slug: scoutrfp-authentication
source_filename: scoutrfp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/scoutrfp-attachments-v1-openapi.json, openapi/scoutrfp-awards-v1-openapi.json,\n  openapi/scoutrfp-contracts-v1-openapi.json, openapi/scoutrfp-events-v1-openapi.json, openapi/scoutrfp-fields-v1-openapi.json,\n  openapi/scoutrfp-payments-v1-openapi.json, openapi/scoutrfp-projects-v1-openapi.json, openapi/scoutrfp-reports-v1-openapi.json,\n  openapi/scoutrfp-scim-v2-openapi.json, openapi/scoutrfp-spend_categories-v1-openapi.json,\n  openapi/scoutrfp-suppliers-v1-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Company API key.\n  sources:\n  - openapi/scoutrfp-attachments-v1-openapi.json\n  - openapi/scoutrfp-awards-v1-openapi.json\n  - openapi/scoutrfp-contracts-v1-openapi.json\n  - openapi/scoutrfp-events-v1-openapi.json\n  - openapi/scoutrfp-fields-v1-openapi.json\n  - openapi/scoutrfp-payments-v1-openapi.json\n\
  \  - openapi/scoutrfp-projects-v1-openapi.json\n  - openapi/scoutrfp-reports-v1-openapi.json\n  - openapi/scoutrfp-scim-v2-openapi.json\n  - openapi/scoutrfp-spend_categories-v1-openapi.json\n  - openapi/scoutrfp-suppliers-v1-openapi.json\n- name: user_token\n  type: apiKey\n  in: header\n  parameter: X-User-Token\n  description: User token.\n  sources:\n  - openapi/scoutrfp-attachments-v1-openapi.json\n  - openapi/scoutrfp-awards-v1-openapi.json\n  - openapi/scoutrfp-contracts-v1-openapi.json\n  - openapi/scoutrfp-events-v1-openapi.json\n  - openapi/scoutrfp-fields-v1-openapi.json\n  - openapi/scoutrfp-payments-v1-openapi.json\n  - openapi/scoutrfp-projects-v1-openapi.json\n  - openapi/scoutrfp-reports-v1-openapi.json\n  - openapi/scoutrfp-spend_categories-v1-openapi.json\n  - openapi/scoutrfp-suppliers-v1-openapi.json\n- name: user_email\n  type: apiKey\n  in: header\n  parameter: X-User-Email\n  description: User email.\n  sources:\n  - openapi/scoutrfp-attachments-v1-openapi.json\n\
  \  - openapi/scoutrfp-awards-v1-openapi.json\n  - openapi/scoutrfp-contracts-v1-openapi.json\n  - openapi/scoutrfp-events-v1-openapi.json\n  - openapi/scoutrfp-fields-v1-openapi.json\n  - openapi/scoutrfp-payments-v1-openapi.json\n  - openapi/scoutrfp-projects-v1-openapi.json\n  - openapi/scoutrfp-reports-v1-openapi.json\n  - openapi/scoutrfp-spend_categories-v1-openapi.json\n  - openapi/scoutrfp-suppliers-v1-openapi.json\n- name: basic_authentication\n  type: http\n  scheme: basic\n  sources:\n  - openapi/scoutrfp-scim-v2-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/authentication/scoutrfp-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Company
- Enterprise
- Procurement
- Strategic Sourcing
- Supplier Management
- Spend Management
- RFP
- Contracts
- SCIM
- JSON:API
---
