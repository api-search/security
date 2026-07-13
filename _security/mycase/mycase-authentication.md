---
api_key_in: []
api_specs:
- filename: mycase-open-api-openapi.yml
  format: yaml
  label: MyCase Open API
  slug: open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mycase/refs/heads/main/openapi/mycase-open-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mycase Authentication
name_suffix: Authentication
oauth_flows: []
overview: MyCase secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MyCase
provider_slug: mycase
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer token issued through the MyCase Open API onboarding flow. The exact authorization endpoint is documented inside the authenticated Stoplight reference.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/mycase-open-api-openapi.yml
  type: http
slug: mycase-authentication
source_filename: mycase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mycase-open-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token issued through the MyCase Open API onboarding flow. The exact authorization\n    endpoint is documented inside the authenticated Stoplight reference.\n  sources:\n  - openapi/mycase-open-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mycase/refs/heads/main/authentication/mycase-authentication.yml
summary_line: http · 1 scheme
tags:
- Billing
- Calendaring
- Case Management
- Client Portal
- Document Management
- Invoicing
- Law Firms
- Legal
- Legal Practice Management
- LegalTech
- Matter Management
- OAuth 2.0
- Payments
- Practice Management
- Time Tracking
- Webhooks
---
