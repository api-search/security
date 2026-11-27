---
anonymous_access: false
api_key_in: []
api_specs:
- filename: paidnice-com-action-api-openapi.yml
  format: yaml
  label: Paidnice Action API
  slug: paidnice-com-action-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidnice-com/openapi/paidnice-com-action-api-openapi.yml
- filename: paidnice-com-contact-api-openapi.yml
  format: yaml
  label: Paidnice Contact API
  slug: paidnice-com-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidnice-com/openapi/paidnice-com-contact-api-openapi.yml
- filename: paidnice-com-inbound-api-openapi.yml
  format: yaml
  label: Paidnice Inbound API
  slug: paidnice-com-inbound-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidnice-com/openapi/paidnice-com-inbound-api-openapi.yml
- filename: paidnice-com-invoice-api-openapi.yml
  format: yaml
  label: Paidnice Invoice API
  slug: paidnice-com-invoice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidnice-com/openapi/paidnice-com-invoice-api-openapi.yml
- filename: paidnice-com-note-api-openapi.yml
  format: yaml
  label: Paidnice Note API
  slug: paidnice-com-note-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidnice-com/openapi/paidnice-com-note-api-openapi.yml
- filename: paidnice-com-organisation-api-openapi.yml
  format: yaml
  label: Paidnice Organisation API
  slug: paidnice-com-organisation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidnice-com/openapi/paidnice-com-organisation-api-openapi.yml
- filename: paidnice-com-stripe-payment-api-openapi.yml
  format: yaml
  label: Paidnice Stripe Payment API
  slug: paidnice-com-stripe-payment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidnice-com/openapi/paidnice-com-stripe-payment-api-openapi.yml
- filename: paidnice-com-user-api-openapi.yml
  format: yaml
  label: Paidnice User API
  slug: paidnice-com-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidnice-com/openapi/paidnice-com-user-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Paidnice Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paidnice secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Paidnice
provider_slug: paidnice-com
scheme_count: 1
schemes:
- description: 'Your Paidnice API key, passed as a bearer token. Tokens carry read and/or write scopes: GET endpoints need read, all other endpoints need write.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/paidnice-com-openapi.json
  type: http
slug: paidnice-com-authentication
source_filename: paidnice-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: derived\nsource: openapi/paidnice-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Your Paidnice API key, passed as a bearer token. Tokens carry read and/or write\n    scopes: GET endpoints need read, all other endpoints need write.'\n  sources:\n  - openapi/paidnice-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/paidnice-com/authentication/paidnice-com-authentication.yml
summary_line: http · 1 scheme
tags:
- AR Automation
- Accounting
- Payments
- Artificial Intelligence
- Software-as-a-Service
---
