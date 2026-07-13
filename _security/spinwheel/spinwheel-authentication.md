---
api_key_in: []
api_specs:
- filename: spinwheel-openapi.yml
  format: yaml
  label: Spinwheel Credit Data API
  slug: credit-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinwheel/refs/heads/main/openapi/spinwheel-openapi.yml
- filename: spinwheel-openapi.yml
  format: yaml
  label: Spinwheel Liabilities & Debt API
  slug: liabilities-debt
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinwheel/refs/heads/main/openapi/spinwheel-openapi.yml
- filename: spinwheel-openapi.yml
  format: yaml
  label: Spinwheel Payments API
  slug: payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinwheel/refs/heads/main/openapi/spinwheel-openapi.yml
- filename: spinwheel-openapi.yml
  format: yaml
  label: Spinwheel Users & Modules API
  slug: users-modules
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinwheel/refs/heads/main/openapi/spinwheel-openapi.yml
- filename: spinwheel-openapi.yml
  format: yaml
  label: Spinwheel Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinwheel/refs/heads/main/openapi/spinwheel-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Spinwheel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spinwheel secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Spinwheel
provider_slug: spinwheel
scheme_count: 1
schemes:
- description: Spinwheel secret API key issued from the developer portal (https://developer.spinwheel.io). The exact transport header is gated behind the developer login and not reconciled here.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/spinwheel-openapi.yml
  type: http
slug: spinwheel-authentication
source_filename: spinwheel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spinwheel-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Spinwheel secret API key issued from the developer portal (https://developer.spinwheel.io).\n    The exact transport header is gated behind the developer login and not reconciled here.\n  sources:\n  - openapi/spinwheel-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spinwheel/refs/heads/main/authentication/spinwheel-authentication.yml
summary_line: http · 1 scheme
tags:
- Fintech
- Credit Data
- Debt
- Liabilities
- Payments
- Embedded Finance
---
