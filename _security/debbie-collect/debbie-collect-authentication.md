---
api_key_in: []
api_specs:
- filename: debbie-platform-api-openapi.yml
  format: yaml
  label: Debbie Platform API
  slug: debbie-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debbie-collect/refs/heads/main/openapi/debbie-platform-api-openapi.yml
- filename: debbie-client-api-openapi.yml
  format: yaml
  label: Debbie Client API
  slug: debbie-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debbie-collect/refs/heads/main/openapi/debbie-client-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Debbie Collect Authentication
name_suffix: Authentication
oauth_flows: []
overview: Debbie Collect secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Debbie Collect
provider_slug: debbie-collect
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/debbie-client-api-openapi.yml
  - openapi/debbie-platform-api-openapi.yml
  type: http
slug: debbie-collect-authentication
source_filename: debbie-collect-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/debbie-client-api-openapi.yml, openapi/debbie-platform-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/debbie-client-api-openapi.yml\n  - openapi/debbie-platform-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/debbie-collect/refs/heads/main/authentication/debbie-collect-authentication.yml
summary_line: http · 1 scheme
tags:
- Accounts Receivable
- Collections
- Debt Collection
- FinTech
- Payments
- SaaS
---
