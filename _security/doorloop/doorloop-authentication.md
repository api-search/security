---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: doorloop-accounts-api-openapi.yml
  format: yaml
  label: DoorLoop Accounts API
  slug: doorloop-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doorloop/refs/heads/main/openapi/doorloop-accounts-api-openapi.yml
- filename: doorloop-communications-api-openapi.yml
  format: yaml
  label: DoorLoop Communications API
  slug: doorloop-communications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doorloop/refs/heads/main/openapi/doorloop-communications-api-openapi.yml
- filename: doorloop-expenses-api-openapi.yml
  format: yaml
  label: DoorLoop Expenses API
  slug: doorloop-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doorloop/refs/heads/main/openapi/doorloop-expenses-api-openapi.yml
- filename: doorloop-files-api-openapi.yml
  format: yaml
  label: DoorLoop Files API
  slug: doorloop-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doorloop/refs/heads/main/openapi/doorloop-files-api-openapi.yml
- filename: doorloop-lease-charges-api-openapi.yml
  format: yaml
  label: DoorLoop Lease Charges API
  slug: doorloop-lease-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doorloop/refs/heads/main/openapi/doorloop-lease-charges-api-openapi.yml
- filename: doorloop-lease-credits-api-openapi.yml
  format: yaml
  label: DoorLoop Lease Credits API
  slug: doorloop-lease-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doorloop/refs/heads/main/openapi/doorloop-lease-credits-api-openapi.yml
- filename: doorloop-lease-payments-api-openapi.yml
  format: yaml
  label: DoorLoop Lease Payments API
  slug: doorloop-lease-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doorloop/refs/heads/main/openapi/doorloop-lease-payments-api-openapi.yml
- filename: doorloop-lease-returned-payments-api-openapi.yml
  format: yaml
  label: DoorLoop Lease Returned Payments API
  slug: doorloop-lease-returned-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doorloop/refs/heads/main/openapi/doorloop-lease-returned-payments-api-openapi.yml
- filename: doorloop-leases-api-openapi.yml
  format: yaml
  label: DoorLoop Leases API
  slug: doorloop-leases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doorloop/refs/heads/main/openapi/doorloop-leases-api-openapi.yml
- filename: doorloop-notes-api-openapi.yml
  format: yaml
  label: DoorLoop Notes API
  slug: doorloop-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doorloop/refs/heads/main/openapi/doorloop-notes-api-openapi.yml
- filename: doorloop-owners-api-openapi.yml
  format: yaml
  label: DoorLoop Owners API
  slug: doorloop-owners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doorloop/refs/heads/main/openapi/doorloop-owners-api-openapi.yml
- filename: doorloop-portfolios-api-openapi.yml
  format: yaml
  label: DoorLoop Portfolios API
  slug: doorloop-portfolios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doorloop/refs/heads/main/openapi/doorloop-portfolios-api-openapi.yml
- filename: doorloop-properties-api-openapi.yml
  format: yaml
  label: DoorLoop Properties API
  slug: doorloop-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doorloop/refs/heads/main/openapi/doorloop-properties-api-openapi.yml
- filename: doorloop-reports-api-openapi.yml
  format: yaml
  label: DoorLoop Reports API
  slug: doorloop-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doorloop/refs/heads/main/openapi/doorloop-reports-api-openapi.yml
- filename: doorloop-tasks-api-openapi.yml
  format: yaml
  label: DoorLoop Tasks API
  slug: doorloop-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doorloop/refs/heads/main/openapi/doorloop-tasks-api-openapi.yml
- filename: doorloop-tenants-api-openapi.yml
  format: yaml
  label: DoorLoop Tenants API
  slug: doorloop-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doorloop/refs/heads/main/openapi/doorloop-tenants-api-openapi.yml
- filename: doorloop-units-api-openapi.yml
  format: yaml
  label: DoorLoop Units API
  slug: doorloop-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doorloop/refs/heads/main/openapi/doorloop-units-api-openapi.yml
- filename: doorloop-users-api-openapi.yml
  format: yaml
  label: DoorLoop Users API
  slug: doorloop-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doorloop/refs/heads/main/openapi/doorloop-users-api-openapi.yml
- filename: doorloop-vendor-bills-api-openapi.yml
  format: yaml
  label: DoorLoop Vendor Bills API
  slug: doorloop-vendor-bills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doorloop/refs/heads/main/openapi/doorloop-vendor-bills-api-openapi.yml
- filename: doorloop-vendor-credits-api-openapi.yml
  format: yaml
  label: DoorLoop Vendor Credits API
  slug: doorloop-vendor-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doorloop/refs/heads/main/openapi/doorloop-vendor-credits-api-openapi.yml
- filename: doorloop-vendors-api-openapi.yml
  format: yaml
  label: DoorLoop Vendors API
  slug: doorloop-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doorloop/refs/heads/main/openapi/doorloop-vendors-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Doorloop Authentication
name_suffix: Authentication
oauth_flows: []
overview: DoorLoop secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DoorLoop
provider_slug: doorloop
scheme_count: 1
schemes:
- description: 'Bearer token. Create a key under Settings -> API access; it is a JWT. Example: `Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.<payload>.<signature>`'
  in: header
  name: Key
  parameter: Authorization
  sources:
  - openapi/doorloop-api-reference-openapi.yml
  type: apiKey
slug: doorloop-authentication
source_filename: doorloop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: derived\nsource: openapi/doorloop-api-reference-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Bearer token. Create a key under Settings -> API access; it is a JWT. Example:\n    `Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.<payload>.<signature>`'\n  sources:\n  - openapi/doorloop-api-reference-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doorloop/refs/heads/main/authentication/doorloop-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Property Management
- Real Estate
- Leases
- Rent Collection
- Maintenance
- Accounting
- Tenant Communication
---
