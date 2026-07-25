---
api_key_in: []
api_specs:
- filename: logikio-blueprint-export-api-openapi.yml
  format: yaml
  label: Logik.io Blueprint > Export API
  slug: logikio-blueprint-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-blueprint-export-api-openapi.yml
- filename: logikio-blueprint-import-api-openapi.yml
  format: yaml
  label: Logik.io Blueprint > Import API
  slug: logikio-blueprint-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-blueprint-import-api-openapi.yml
- filename: logikio-bom-api-openapi.yml
  format: yaml
  label: Logik.io BOM API
  slug: logikio-bom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-bom-api-openapi.yml
- filename: logikio-configuration-api-openapi.yml
  format: yaml
  label: Logik.io Configuration API
  slug: logikio-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-configuration-api-openapi.yml
- filename: logikio-configuration-v2-api-openapi.yml
  format: yaml
  label: Logik.io Configuration (V2) API
  slug: logikio-configuration-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-configuration-v2-api-openapi.yml
- filename: logikio-managed-tables-export-tables-api-openapi.yml
  format: yaml
  label: Logik.io Managed Tables > Export Tables API
  slug: logikio-managed-tables-export-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-managed-tables-export-tables-api-openapi.yml
- filename: logikio-managed-tables-import-tables-api-openapi.yml
  format: yaml
  label: Logik.io Managed Tables > Import Tables API
  slug: logikio-managed-tables-import-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-managed-tables-import-tables-api-openapi.yml
- filename: logikio-managed-tables-metadata-api-openapi.yml
  format: yaml
  label: Logik.io Managed Tables > Metadata API
  slug: logikio-managed-tables-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-managed-tables-metadata-api-openapi.yml
- filename: logikio-managed-tables-table-rows-api-openapi.yml
  format: yaml
  label: Logik.io Managed Tables > Table Rows API
  slug: logikio-managed-tables-table-rows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-managed-tables-table-rows-api-openapi.yml
- filename: logikio-managed-tables-tables-api-openapi.yml
  format: yaml
  label: Logik.io Managed Tables > Tables API
  slug: logikio-managed-tables-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-managed-tables-tables-api-openapi.yml
- filename: logikio-runtime-bill-of-materials-api-openapi.yml
  format: yaml
  label: Logik.io Runtime - Bill of Materials API
  slug: logikio-runtime-bill-of-materials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-runtime-bill-of-materials-api-openapi.yml
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
