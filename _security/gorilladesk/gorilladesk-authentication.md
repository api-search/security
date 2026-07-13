---
api_key_in: []
api_specs:
- filename: gorilladesk-openapi.yml
  format: yaml
  label: GorillaDesk Customers API
  slug: gorilladesk-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorilladesk/refs/heads/main/openapi/gorilladesk-openapi.yml
- filename: gorilladesk-openapi.yml
  format: yaml
  label: GorillaDesk Customer Notes API
  slug: gorilladesk-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorilladesk/refs/heads/main/openapi/gorilladesk-openapi.yml
- filename: gorilladesk-openapi.yml
  format: yaml
  label: GorillaDesk Users API
  slug: gorilladesk-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorilladesk/refs/heads/main/openapi/gorilladesk-openapi.yml
- filename: gorilladesk-openapi.yml
  format: yaml
  label: GorillaDesk Company API
  slug: gorilladesk-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorilladesk/refs/heads/main/openapi/gorilladesk-openapi.yml
- filename: gorilladesk-openapi.yml
  format: yaml
  label: GorillaDesk Phone Types API
  slug: gorilladesk-phone-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorilladesk/refs/heads/main/openapi/gorilladesk-openapi.yml
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
