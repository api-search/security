---
api_key_in: []
api_specs:
- filename: zylo-applications-api-openapi.yml
  format: yaml
  label: Zylo Applications API
  slug: zylo-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zylo/refs/heads/main/openapi/zylo-applications-api-openapi.yml
- filename: zylo-export-jobs-api-openapi.yml
  format: yaml
  label: Zylo Export Jobs API
  slug: zylo-export-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zylo/refs/heads/main/openapi/zylo-export-jobs-api-openapi.yml
- filename: zylo-import-jobs-api-openapi.yml
  format: yaml
  label: Zylo Import Jobs API
  slug: zylo-import-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zylo/refs/heads/main/openapi/zylo-import-jobs-api-openapi.yml
- filename: zylo-subscriptions-api-openapi.yml
  format: yaml
  label: Zylo Subscriptions API
  slug: zylo-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zylo/refs/heads/main/openapi/zylo-subscriptions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Zylo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zylo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zylo
provider_slug: zylo
scheme_count: 1
schemes:
- description: Bearer token authentication using your Token ID and Token Secret separated by a colon (TOKENID:TOKENSECRET). Tokens can be created in the Zylo Admin panel under Company Tokens.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/zylo-enterprise-openapi.yml
  type: http
slug: zylo-authentication
source_filename: zylo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zylo-enterprise-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication using your Token ID and Token Secret separated by\n    a colon (TOKENID:TOKENSECRET). Tokens can be created in the Zylo Admin panel under Company\n    Tokens.\n  sources:\n  - openapi/zylo-enterprise-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zylo/refs/heads/main/authentication/zylo-authentication.yml
summary_line: http · 1 scheme
tags:
- Budgets
- SaaS Management
- Spend
---
