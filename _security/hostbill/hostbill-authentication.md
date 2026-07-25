---
api_key_in:
- query
api_specs:
- filename: hostbill-accounts-api-openapi.yml
  format: yaml
  label: HostBill Accounts API
  slug: hostbill-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostbill/refs/heads/main/openapi/hostbill-accounts-api-openapi.yml
- filename: hostbill-admin-api-openapi.yml
  format: yaml
  label: HostBill Admin API
  slug: hostbill-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostbill/refs/heads/main/openapi/hostbill-admin-api-openapi.yml
- filename: hostbill-clients-api-openapi.yml
  format: yaml
  label: HostBill Clients API
  slug: hostbill-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostbill/refs/heads/main/openapi/hostbill-clients-api-openapi.yml
- filename: hostbill-domains-api-openapi.yml
  format: yaml
  label: HostBill Domains API
  slug: hostbill-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostbill/refs/heads/main/openapi/hostbill-domains-api-openapi.yml
- filename: hostbill-invoices-api-openapi.yml
  format: yaml
  label: HostBill Invoices API
  slug: hostbill-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostbill/refs/heads/main/openapi/hostbill-invoices-api-openapi.yml
- filename: hostbill-orders-api-openapi.yml
  format: yaml
  label: HostBill Orders API
  slug: hostbill-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostbill/refs/heads/main/openapi/hostbill-orders-api-openapi.yml
- filename: hostbill-tickets-api-openapi.yml
  format: yaml
  label: HostBill Tickets API
  slug: hostbill-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostbill/refs/heads/main/openapi/hostbill-tickets-api-openapi.yml
- filename: hostbill-transactions-api-openapi.yml
  format: yaml
  label: HostBill Transactions API
  slug: hostbill-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostbill/refs/heads/main/openapi/hostbill-transactions-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Hostbill Authentication
name_suffix: Authentication
oauth_flows: []
overview: HostBill secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: HostBill
provider_slug: hostbill
scheme_count: 2
schemes:
- in: query
  name: apiKeyId
  parameter: api_id
  sources:
  - openapi/hostbill-openapi.yml
  type: apiKey
- in: query
  name: apiKeySecret
  parameter: api_key
  sources:
  - openapi/hostbill-openapi.yml
  type: apiKey
slug: hostbill-authentication
source_filename: hostbill-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hostbill-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyId\n  type: apiKey\n  in: query\n  parameter: api_id\n  sources:\n  - openapi/hostbill-openapi.yml\n- name: apiKeySecret\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/hostbill-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hostbill/refs/heads/main/authentication/hostbill-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Automation
- Billing
- Domain Registration
- Web Hosting
---
