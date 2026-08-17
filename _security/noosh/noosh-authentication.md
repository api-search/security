---
api_key_in: []
api_specs:
- filename: noosh-openapi.yml
  format: yaml
  label: Noosh API
  slug: noosh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noosh/refs/heads/main/openapi/noosh-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Noosh Authentication
name_suffix: Authentication
oauth_flows: []
overview: Noosh secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Noosh
provider_slug: noosh
scheme_count: 1
schemes:
- name: HTTP_BASIC
  scheme: basic
  sources:
  - openapi/noosh-openapi.yml
  type: http
slug: noosh-authentication
source_filename: noosh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/noosh-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTP_BASIC\n  type: http\n  scheme: basic\n  sources:\n  - openapi/noosh-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noosh/refs/heads/main/authentication/noosh-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Marketing
- Marketing Execution
- Procurement
- Print
- Direct Mail
- Workflow
- Sourcing
- Print Procurement
- Project Management
- Supplier Management
- Quotes
- Purchase Orders
- Shipments
- Invoicing
---
