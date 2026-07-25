---
api_key_in: []
api_specs:
- filename: arcadia-auth-api-openapi.yml
  format: yaml
  label: Arcadia Auth API
  slug: arcadia-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadia/refs/heads/main/openapi/arcadia-auth-api-openapi.yml
- filename: arcadia-bundle-beta-api-openapi.yml
  format: yaml
  label: Arcadia Bundle (Beta) API
  slug: arcadia-bundle-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadia/refs/heads/main/openapi/arcadia-bundle-beta-api-openapi.yml
- filename: arcadia-plug-api-openapi.yml
  format: yaml
  label: Arcadia Plug API
  slug: arcadia-plug-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadia/refs/heads/main/openapi/arcadia-plug-api-openapi.yml
- filename: arcadia-spark-api-openapi.yml
  format: yaml
  label: Arcadia Spark API
  slug: arcadia-spark-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadia/refs/heads/main/openapi/arcadia-spark-api-openapi.yml
- filename: arcadia-users-api-openapi.yml
  format: yaml
  label: Arcadia Users API
  slug: arcadia-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadia/refs/heads/main/openapi/arcadia-users-api-openapi.yml
- filename: arcadia-utility-accounts-api-openapi.yml
  format: yaml
  label: Arcadia Utility Accounts API
  slug: arcadia-utility-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadia/refs/heads/main/openapi/arcadia-utility-accounts-api-openapi.yml
- filename: arcadia-utility-credentials-api-openapi.yml
  format: yaml
  label: Arcadia Utility Credentials API
  slug: arcadia-utility-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadia/refs/heads/main/openapi/arcadia-utility-credentials-api-openapi.yml
- filename: arcadia-utility-meters-beta-api-openapi.yml
  format: yaml
  label: Arcadia Utility Meters (Beta) API
  slug: arcadia-utility-meters-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadia/refs/heads/main/openapi/arcadia-utility-meters-beta-api-openapi.yml
- filename: arcadia-webhooks-api-openapi.yml
  format: yaml
  label: Arcadia Webhooks API
  slug: arcadia-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadia/refs/heads/main/openapi/arcadia-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Arcadia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arcadia secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Arcadia
provider_slug: arcadia
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/arcadia-plug-openapi.yml
  type: http
slug: arcadia-authentication
source_filename: arcadia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/arcadia-plug-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/arcadia-plug-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arcadia/refs/heads/main/authentication/arcadia-authentication.yml
summary_line: http · 1 scheme
tags:
- Energy
- Utilities
- Clean Energy
- Billing Data
- Interval Data
- Carbon
- Solar
- Tariff
---
