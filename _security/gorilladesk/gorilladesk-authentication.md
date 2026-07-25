---
api_key_in: []
api_specs:
- filename: gorilladesk-company-api-openapi.yml
  format: yaml
  label: GorillaDesk Company API
  slug: gorilladesk-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorilladesk/refs/heads/main/openapi/gorilladesk-company-api-openapi.yml
- filename: gorilladesk-customer-api-openapi.yml
  format: yaml
  label: GorillaDesk Customer API
  slug: gorilladesk-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorilladesk/refs/heads/main/openapi/gorilladesk-customer-api-openapi.yml
- filename: gorilladesk-note-api-openapi.yml
  format: yaml
  label: GorillaDesk Note API
  slug: gorilladesk-note-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorilladesk/refs/heads/main/openapi/gorilladesk-note-api-openapi.yml
- filename: gorilladesk-phone-type-api-openapi.yml
  format: yaml
  label: GorillaDesk Phone Type API
  slug: gorilladesk-phone-type-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorilladesk/refs/heads/main/openapi/gorilladesk-phone-type-api-openapi.yml
- filename: gorilladesk-user-api-openapi.yml
  format: yaml
  label: GorillaDesk User API
  slug: gorilladesk-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorilladesk/refs/heads/main/openapi/gorilladesk-user-api-openapi.yml
- filename: gorilladesk-users-api-openapi.yml
  format: yaml
  label: GorillaDesk Users API
  slug: gorilladesk-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorilladesk/refs/heads/main/openapi/gorilladesk-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gorilladesk Authentication
name_suffix: Authentication
oauth_flows: []
overview: GorillaDesk secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GorillaDesk
provider_slug: gorilladesk
scheme_count: 1
schemes:
- name: Bearer
  scheme: bearer
  sources:
  - openapi/gorilladesk-openapi.yml
  type: http
slug: gorilladesk-authentication
source_filename: gorilladesk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gorilladesk-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/gorilladesk-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gorilladesk/refs/heads/main/authentication/gorilladesk-authentication.yml
summary_line: http · 1 scheme
tags:
- Field Service Management
- Pest Control
- Lawn Care
- Scheduling
- Invoicing
- Customers
- SaaS
---
