---
api_key_in: []
api_specs:
- filename: avaloq-banking-openapi.yml
  format: yaml
  label: Avaloq Banking API
  slug: avaloq-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/openapi/avaloq-banking-openapi.yml
- filename: avaloq-wealth-management-openapi.yml
  format: yaml
  label: Avaloq Wealth Management API
  slug: avaloq-wealth-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/openapi/avaloq-wealth-management-openapi.yml
- filename: avaloq-payments-openapi.yml
  format: yaml
  label: Avaloq Payments API
  slug: avaloq-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/openapi/avaloq-payments-openapi.yml
- filename: avaloq-client-management-openapi.yml
  format: yaml
  label: Avaloq Client Management API
  slug: avaloq-client-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/openapi/avaloq-client-management-openapi.yml
- filename: avaloq-trading-openapi.yml
  format: yaml
  label: Avaloq Trading API
  slug: avaloq-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/openapi/avaloq-trading-openapi.yml
- filename: avaloq-compliance-openapi.yml
  format: yaml
  label: Avaloq Compliance & Risk API
  slug: avaloq-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/openapi/avaloq-compliance-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Avaloq Authentication
name_suffix: Authentication
oauth_flows: []
overview: Avaloq secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Avaloq
provider_slug: avaloq
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/avaloq-banking-openapi.yml
  - openapi/avaloq-payments-openapi.yml
  type: http
slug: avaloq-authentication
source_filename: avaloq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/avaloq-banking-openapi.yml, openapi/avaloq-payments-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/avaloq-banking-openapi.yml\n  - openapi/avaloq-payments-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/authentication/avaloq-authentication.yml
summary_line: http · 1 scheme
tags:
- Banking
- Digital Banking
- Financial Services
- Fintech
- Payments
- Wealth Management
---
