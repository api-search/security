---
api_key_in:
- header
api_specs:
- filename: customeros-openapi.yml
  format: yaml
  label: CustomerOS GraphQL Core API
  slug: customeros-graphql-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customeros/refs/heads/main/openapi/customeros-openapi.yml
- filename: customeros-openapi.yml
  format: yaml
  label: CustomerOS Organizations API
  slug: customeros-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customeros/refs/heads/main/openapi/customeros-openapi.yml
- filename: customeros-openapi.yml
  format: yaml
  label: CustomerOS Contacts API
  slug: customeros-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customeros/refs/heads/main/openapi/customeros-openapi.yml
- filename: customeros-openapi.yml
  format: yaml
  label: CustomerOS Opportunities API
  slug: customeros-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customeros/refs/heads/main/openapi/customeros-openapi.yml
- filename: customeros-openapi.yml
  format: yaml
  label: CustomerOS Interactions API
  slug: customeros-interactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customeros/refs/heads/main/openapi/customeros-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Customeros Authentication
name_suffix: Authentication
oauth_flows: []
overview: CustomerOS secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CustomerOS
provider_slug: customeros
scheme_count: 1
schemes:
- description: Per-tenant API key. The open-source customer-os-api validates an API key header and resolves the tenant before applying @hasRole / @hasTenant directives. Header name and exact auth flow depend on deployment; the documented customeros.ai cloud REST surface uses X-CUSTOMER-OS-API-KEY.
  in: header
  name: ApiKeyAuth
  parameter: X-Openline-API-KEY
  sources:
  - openapi/customeros-openapi.yml
  type: apiKey
slug: customeros-authentication
source_filename: customeros-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/customeros-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Openline-API-KEY\n  description: Per-tenant API key. The open-source customer-os-api validates an API key header\n    and resolves the tenant before applying @hasRole / @hasTenant directives. Header name and\n    exact auth flow depend on deployment; the documented customeros.ai cloud REST surface uses\n    X-CUSTOMER-OS-API-KEY.\n  sources:\n  - openapi/customeros-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/customeros/refs/heads/main/authentication/customeros-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- CRM
- Revenue
- Go-To-Market
- GraphQL
- Open Source
---
