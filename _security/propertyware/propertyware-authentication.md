---
api_key_in:
- header
api_specs:
- filename: propertyware-accounting-api-openapi.yml
  format: yaml
  label: Propertyware Accounting API
  slug: propertyware-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-accounting-api-openapi.yml
- filename: propertyware-bills-api-openapi.yml
  format: yaml
  label: Propertyware Bills API
  slug: propertyware-bills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-bills-api-openapi.yml
- filename: propertyware-buildings-api-openapi.yml
  format: yaml
  label: Propertyware Buildings API
  slug: propertyware-buildings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-buildings-api-openapi.yml
- filename: propertyware-contacts-api-openapi.yml
  format: yaml
  label: Propertyware Contacts API
  slug: propertyware-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-contacts-api-openapi.yml
- filename: propertyware-custom-field-definitions-api-openapi.yml
  format: yaml
  label: Propertyware Custom field definitions API
  slug: propertyware-custom-field-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-custom-field-definitions-api-openapi.yml
- filename: propertyware-documents-api-openapi.yml
  format: yaml
  label: Propertyware Documents API
  slug: propertyware-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-documents-api-openapi.yml
- filename: propertyware-health-check-api-openapi.yml
  format: yaml
  label: Propertyware Health check API
  slug: propertyware-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-health-check-api-openapi.yml
- filename: propertyware-inspections-api-openapi.yml
  format: yaml
  label: Propertyware Inspections API
  slug: propertyware-inspections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-inspections-api-openapi.yml
- filename: propertyware-leases-api-openapi.yml
  format: yaml
  label: Propertyware Leases API
  slug: propertyware-leases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-leases-api-openapi.yml
- filename: propertyware-portfolios-api-openapi.yml
  format: yaml
  label: Propertyware Portfolios API
  slug: propertyware-portfolios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-portfolios-api-openapi.yml
- filename: propertyware-prospects-api-openapi.yml
  format: yaml
  label: Propertyware Prospects API
  slug: propertyware-prospects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-prospects-api-openapi.yml
- filename: propertyware-units-api-openapi.yml
  format: yaml
  label: Propertyware Units API
  slug: propertyware-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-units-api-openapi.yml
- filename: propertyware-vendors-api-openapi.yml
  format: yaml
  label: Propertyware Vendors API
  slug: propertyware-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-vendors-api-openapi.yml
- filename: propertyware-work-orders-api-openapi.yml
  format: yaml
  label: Propertyware Work orders API
  slug: propertyware-work-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-work-orders-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Propertyware Authentication
name_suffix: Authentication
oauth_flows: []
overview: Propertyware secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Propertyware
provider_slug: propertyware
scheme_count: 3
schemes:
- in: header
  name: clientId
  parameter: x-propertyware-client-id
  sources:
  - openapi/propertyware-openapi.json
  type: apiKey
- in: header
  name: clientSecret
  parameter: x-propertyware-client-secret
  sources:
  - openapi/propertyware-openapi.json
  type: apiKey
- in: header
  name: organizationId
  parameter: x-propertyware-system-id
  sources:
  - openapi/propertyware-openapi.json
  type: apiKey
slug: propertyware-authentication
source_filename: propertyware-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/propertyware-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: clientId\n  type: apiKey\n  in: header\n  parameter: x-propertyware-client-id\n  sources:\n  - openapi/propertyware-openapi.json\n- name: clientSecret\n  type: apiKey\n  in: header\n  parameter: x-propertyware-client-secret\n  sources:\n  - openapi/propertyware-openapi.json\n- name: organizationId\n  type: apiKey\n  in: header\n  parameter: x-propertyware-system-id\n  sources:\n  - openapi/propertyware-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/authentication/propertyware-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Property Management
- Real-Estate
- Rental Properties
- Single-Family Rentals
- Leases
- Tenants
- Maintenance
- Work Orders
- Financial Transactions
- Owner Reports
---
