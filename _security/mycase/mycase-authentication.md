---
api_key_in: []
api_specs:
- filename: mycase-case-stages-api-openapi.yml
  format: yaml
  label: MyCase Case Stages API
  slug: mycase-case-stages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mycase/refs/heads/main/openapi/mycase-case-stages-api-openapi.yml
- filename: mycase-cases-api-openapi.yml
  format: yaml
  label: MyCase Cases API
  slug: mycase-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mycase/refs/heads/main/openapi/mycase-cases-api-openapi.yml
- filename: mycase-companies-api-openapi.yml
  format: yaml
  label: MyCase Companies API
  slug: mycase-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mycase/refs/heads/main/openapi/mycase-companies-api-openapi.yml
- filename: mycase-contacts-api-openapi.yml
  format: yaml
  label: MyCase Contacts API
  slug: mycase-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mycase/refs/heads/main/openapi/mycase-contacts-api-openapi.yml
- filename: mycase-documents-api-openapi.yml
  format: yaml
  label: MyCase Documents API
  slug: mycase-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mycase/refs/heads/main/openapi/mycase-documents-api-openapi.yml
- filename: mycase-events-api-openapi.yml
  format: yaml
  label: MyCase Events API
  slug: mycase-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mycase/refs/heads/main/openapi/mycase-events-api-openapi.yml
- filename: mycase-firm-api-openapi.yml
  format: yaml
  label: MyCase Firm API
  slug: mycase-firm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mycase/refs/heads/main/openapi/mycase-firm-api-openapi.yml
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
- Document-Management
- Invoicing
- Law Firms
- Legal
- Legal Practice Management
- Legal Tech
- Matter Management
- Authentication
- Payments
- Practice Management
- Time Tracking
- Webhook
---
