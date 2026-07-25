---
api_key_in: []
api_specs:
- filename: waste-management-cases-api-openapi.yml
  format: yaml
  label: Waste Management Cases API
  slug: waste-management-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/waste-management/refs/heads/main/openapi/waste-management-cases-api-openapi.yml
- filename: waste-management-contacts-api-openapi.yml
  format: yaml
  label: Waste Management Contacts API
  slug: waste-management-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/waste-management/refs/heads/main/openapi/waste-management-contacts-api-openapi.yml
- filename: waste-management-customers-api-openapi.yml
  format: yaml
  label: Waste Management Customers API
  slug: waste-management-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/waste-management/refs/heads/main/openapi/waste-management-customers-api-openapi.yml
- filename: waste-management-invoices-api-openapi.yml
  format: yaml
  label: Waste Management Invoices API
  slug: waste-management-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/waste-management/refs/heads/main/openapi/waste-management-invoices-api-openapi.yml
- filename: waste-management-preferences-api-openapi.yml
  format: yaml
  label: Waste Management Preferences API
  slug: waste-management-preferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/waste-management/refs/heads/main/openapi/waste-management-preferences-api-openapi.yml
- filename: waste-management-services-api-openapi.yml
  format: yaml
  label: Waste Management Services API
  slug: waste-management-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/waste-management/refs/heads/main/openapi/waste-management-services-api-openapi.yml
- filename: waste-management-tickets-api-openapi.yml
  format: yaml
  label: Waste Management Tickets API
  slug: waste-management-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/waste-management/refs/heads/main/openapi/waste-management-tickets-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Waste Management Authentication
name_suffix: Authentication
oauth_flows: []
overview: Waste Management secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Waste Management
provider_slug: waste-management
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JSON Web Token (JWT) provided by WM.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/waste-management-customer-api-openapi.yml
  type: http
slug: waste-management-authentication
source_filename: waste-management-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/waste-management-customer-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JSON Web Token (JWT) provided by WM.\n  sources:\n  - openapi/waste-management-customer-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/waste-management/refs/heads/main/authentication/waste-management-authentication.yml
summary_line: http · 1 scheme
tags:
- Environmental Services
- Fortune 500
- Recycling
- Solid Waste
- Sustainability
- Waste Management
---
