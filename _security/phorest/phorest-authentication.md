---
api_key_in: []
api_specs:
- filename: phorest-appointments-api-openapi.yml
  format: yaml
  label: Phorest Appointments API
  slug: phorest-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-appointments-api-openapi.yml
- filename: phorest-bookings-api-openapi.yml
  format: yaml
  label: Phorest Bookings API
  slug: phorest-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-bookings-api-openapi.yml
- filename: phorest-branches-api-openapi.yml
  format: yaml
  label: Phorest Branches API
  slug: phorest-branches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-branches-api-openapi.yml
- filename: phorest-clients-api-openapi.yml
  format: yaml
  label: Phorest Clients API
  slug: phorest-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-clients-api-openapi.yml
- filename: phorest-courses-api-openapi.yml
  format: yaml
  label: Phorest Courses API
  slug: phorest-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-courses-api-openapi.yml
- filename: phorest-leads-api-openapi.yml
  format: yaml
  label: Phorest Leads API
  slug: phorest-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-leads-api-openapi.yml
- filename: phorest-loyalty-api-openapi.yml
  format: yaml
  label: Phorest Loyalty API
  slug: phorest-loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-loyalty-api-openapi.yml
- filename: phorest-products-api-openapi.yml
  format: yaml
  label: Phorest Products API
  slug: phorest-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-products-api-openapi.yml
- filename: phorest-purchases-api-openapi.yml
  format: yaml
  label: Phorest Purchases API
  slug: phorest-purchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-purchases-api-openapi.yml
- filename: phorest-reporting-api-openapi.yml
  format: yaml
  label: Phorest Reporting API
  slug: phorest-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-reporting-api-openapi.yml
- filename: phorest-reviews-api-openapi.yml
  format: yaml
  label: Phorest Reviews API
  slug: phorest-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-reviews-api-openapi.yml
- filename: phorest-services-api-openapi.yml
  format: yaml
  label: Phorest Services API
  slug: phorest-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-services-api-openapi.yml
- filename: phorest-staff-api-openapi.yml
  format: yaml
  label: Phorest Staff API
  slug: phorest-staff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-staff-api-openapi.yml
- filename: phorest-vouchers-api-openapi.yml
  format: yaml
  label: Phorest Vouchers API
  slug: phorest-vouchers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-vouchers-api-openapi.yml
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
