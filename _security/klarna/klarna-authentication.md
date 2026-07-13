---
api_key_in: []
api_specs:
- filename: klarna-payments-api-openapi.yml
  format: yaml
  label: Klarna Payments API
  slug: klarna-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-payments-api-openapi.yml
- filename: klarna-customer-token-api-openapi.yml
  format: yaml
  label: Klarna Customer Token API
  slug: klarna-customer-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-customer-token-api-openapi.yml
- filename: klarna-settlements-api-openapi.yml
  format: yaml
  label: Klarna Settlements API
  slug: klarna-settlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-settlements-api-openapi.yml
- filename: klarna-push-notifications-asyncapi.yml
  format: yaml
  label: Klarna Push Notifications
  slug: klarna-push-notifications
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/asyncapi/klarna-push-notifications-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Klarna Authentication
name_suffix: Authentication
oauth_flows: []
overview: Klarna secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Klarna
provider_slug: klarna
scheme_count: 1
schemes:
- name: basic_auth
  scheme: basic
  sources:
  - openapi/klarna-settlements-api-openapi.yml
  - openapi/order-management-api-openapi.yml
  type: http
slug: klarna-authentication
source_filename: klarna-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/klarna-settlements-api-openapi.yml, openapi/order-management-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basic_auth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/klarna-settlements-api-openapi.yml\n  - openapi/order-management-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/authentication/klarna-authentication.yml
summary_line: http · 1 scheme
tags:
- Fintech
- BNPL
- Payments
- Cards
- Shopping
---
