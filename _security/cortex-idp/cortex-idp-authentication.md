---
api_key_in: []
api_specs:
- filename: cortex-idp-openapi.yml
  format: yaml
  label: Cortex Catalog API
  slug: cortex-idp-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cortex-idp/refs/heads/main/openapi/cortex-idp-openapi.yml
- filename: cortex-idp-openapi.yml
  format: yaml
  label: Cortex Scorecards API
  slug: cortex-idp-scorecards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cortex-idp/refs/heads/main/openapi/cortex-idp-openapi.yml
- filename: cortex-idp-openapi.yml
  format: yaml
  label: Cortex Custom Data API
  slug: cortex-idp-custom-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cortex-idp/refs/heads/main/openapi/cortex-idp-openapi.yml
- filename: cortex-idp-openapi.yml
  format: yaml
  label: Cortex Initiatives API
  slug: cortex-idp-initiatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cortex-idp/refs/heads/main/openapi/cortex-idp-openapi.yml
- filename: cortex-idp-openapi.yml
  format: yaml
  label: Cortex Deploys API
  slug: cortex-idp-deploys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cortex-idp/refs/heads/main/openapi/cortex-idp-openapi.yml
- filename: cortex-idp-openapi.yml
  format: yaml
  label: Cortex Integrations API
  slug: cortex-idp-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cortex-idp/refs/heads/main/openapi/cortex-idp-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cortex Idp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cortex secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cortex
provider_slug: cortex-idp
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'API key created in the Settings page of your Cortex workspace. Passed as `Authorization: Bearer YOUR_API_KEY`. Cortex API keys are scoped by role and permissions; some operations require specific permissions such as "Edit entities" or "Configure integrations".'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://docs.cortex.io/api
  - openapi/cortex-idp-openapi.yml
  type: http
slug: cortex-idp-authentication
source_filename: cortex-idp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cortex-idp-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'API key created in the Settings page of your Cortex workspace. Passed\n    as `Authorization: Bearer YOUR_API_KEY`. Cortex API keys are scoped by role and\n    permissions; some operations require specific permissions such as \"Edit entities\"\n    or \"Configure integrations\".'\n  sources:\n  - https://docs.cortex.io/api\n  - openapi/cortex-idp-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cortex-idp/refs/heads/main/authentication/cortex-idp-authentication.yml
summary_line: http · 1 scheme
tags:
- Software Catalog
- Internal Developer Portal
- Service Catalog
- Developer Experience
- IDP
- Scorecards
- Platform Engineering
- Developer Portal
---
