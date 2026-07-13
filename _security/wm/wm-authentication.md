---
api_key_in: []
api_specs:
- filename: wm-openapi.yml
  format: yaml
  label: WM Services API
  slug: wm-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wm/refs/heads/main/openapi/wm-openapi.yml
- filename: wm-openapi.yml
  format: yaml
  label: WM Service Operations & Materials API
  slug: wm-service-operations-materials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wm/refs/heads/main/openapi/wm-openapi.yml
- filename: wm-openapi.yml
  format: yaml
  label: WM Service Pricing API
  slug: wm-service-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wm/refs/heads/main/openapi/wm-openapi.yml
- filename: wm-openapi.yml
  format: yaml
  label: WM Invoices & Balance API
  slug: wm-invoices-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wm/refs/heads/main/openapi/wm-openapi.yml
- filename: wm-openapi.yml
  format: yaml
  label: WM Profiles & Preferences API
  slug: wm-profiles-preferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wm/refs/heads/main/openapi/wm-openapi.yml
- filename: wm-openapi.yml
  format: yaml
  label: WM Contacts API
  slug: wm-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wm/refs/heads/main/openapi/wm-openapi.yml
- filename: wm-openapi.yml
  format: yaml
  label: WM Cases & Tickets API
  slug: wm-cases-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wm/refs/heads/main/openapi/wm-openapi.yml
- filename: wm-openapi.yml
  format: yaml
  label: WM Activities API
  slug: wm-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wm/refs/heads/main/openapi/wm-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Wm Authentication
name_suffix: Authentication
oauth_flows: []
overview: WM secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: WM
provider_slug: wm
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: WM issues a JSON Web Token (JWT) and a ClientId to approved partners/customers. Send the token in the Authorization header and the ClientId in the ClientId header on every request.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/wm-openapi.yml
  type: http
slug: wm-authentication
source_filename: wm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wm-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: WM issues a JSON Web Token (JWT) and a ClientId to approved partners/customers.\n    Send the token in the Authorization header and the ClientId in the ClientId header on every\n    request.\n  sources:\n  - openapi/wm-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wm/refs/heads/main/authentication/wm-authentication.yml
summary_line: http · 1 scheme
tags:
- Waste Management
- Recycling
- Environmental Services
- Field Services
- Logistics
- Account Management
- Enterprise
- B2B
---
