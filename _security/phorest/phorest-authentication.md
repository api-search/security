---
api_key_in: []
api_specs:
- filename: phorest-openapi.yml
  format: yaml
  label: Phorest Clients API
  slug: phorest-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-openapi.yml
- filename: phorest-openapi.yml
  format: yaml
  label: Phorest Appointments & Bookings API
  slug: phorest-appointments-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-openapi.yml
- filename: phorest-openapi.yml
  format: yaml
  label: Phorest Staff API
  slug: phorest-staff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-openapi.yml
- filename: phorest-openapi.yml
  format: yaml
  label: Phorest Services API
  slug: phorest-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-openapi.yml
- filename: phorest-openapi.yml
  format: yaml
  label: Phorest Products & Purchases API
  slug: phorest-products-purchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-openapi.yml
- filename: phorest-openapi.yml
  format: yaml
  label: Phorest Vouchers & Loyalty API
  slug: phorest-vouchers-loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-openapi.yml
- filename: phorest-openapi.yml
  format: yaml
  label: Phorest Branches API
  slug: phorest-branches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-openapi.yml
- filename: phorest-openapi.yml
  format: yaml
  label: Phorest Reporting & Reviews API
  slug: phorest-reporting-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Phorest Authentication
name_suffix: Authentication
oauth_flows: []
overview: Phorest secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Phorest
provider_slug: phorest
scheme_count: 1
schemes:
- description: Username is `global/{email}`, using the email address Phorest associated with the granted API access. Password is the API password issued by Phorest support.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/phorest-openapi.yml
  type: http
slug: phorest-authentication
source_filename: phorest-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/phorest-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Username is `global/{email}`, using the email address Phorest associated with\n    the granted API access. Password is the API password issued by Phorest support.\n  sources:\n  - openapi/phorest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/authentication/phorest-authentication.yml
summary_line: http · 1 scheme
tags:
- Salon Software
- Spa Software
- Scheduling
- Point of Sale
- Business Management
- Vertical SaaS
---
