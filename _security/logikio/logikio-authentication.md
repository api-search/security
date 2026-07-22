---
api_key_in: []
api_specs:
- filename: logikio-runtime-v2-openapi-original.yml
  format: yaml
  label: Logik Configurator Runtime API (v2)
  slug: logik-configurator-runtime-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-runtime-v2-openapi-original.yml
- filename: logikio-runtime-v1-openapi-original.yml
  format: yaml
  label: Logik Configurator Runtime API (v1)
  slug: logik-configurator-runtime-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-runtime-v1-openapi-original.yml
- filename: logikio-admin-managed-tables-openapi-original.yml
  format: yaml
  label: Logik.io Admin API - Managed Tables
  slug: logikio-admin-api-managed-tables
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-admin-managed-tables-openapi-original.yml
- filename: logikio-admin-blueprint-openapi-original.yml
  format: yaml
  label: Logik.io Admin API - Blueprint Import/Export
  slug: logikio-admin-api-blueprint-importexport
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-admin-blueprint-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Logikio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Logik.io secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Logik.io
provider_slug: logikio
scheme_count: 1
schemes:
- description: Admin API Bearer Token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/logikio-admin-blueprint-openapi-original.yml
  - openapi/logikio-admin-managed-tables-openapi-original.yml
  - openapi/logikio-runtime-v1-openapi-original.yml
  - openapi/logikio-runtime-v2-openapi-original.yml
  type: http
slug: logikio-authentication
source_filename: logikio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/logikio-admin-blueprint-openapi-original.yml, openapi/logikio-admin-managed-tables-openapi-original.yml,\n  openapi/logikio-runtime-v1-openapi-original.yml, openapi/logikio-runtime-v2-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Admin API Bearer Token\n  sources:\n  - openapi/logikio-admin-blueprint-openapi-original.yml\n  - openapi/logikio-admin-managed-tables-openapi-original.yml\n  - openapi/logikio-runtime-v1-openapi-original.yml\n  - openapi/logikio-runtime-v2-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/authentication/logikio-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Sales Tech
- CPQ
- Configure Price Quote
- Product Configuration
- Bill of Materials
- Ecommerce
- Salesforce
- API-First
---
