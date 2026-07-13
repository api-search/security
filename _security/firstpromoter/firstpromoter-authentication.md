---
api_key_in: []
api_specs:
- filename: firstpromoter-firstpromoter-admin-api-openapi.yml
  format: yaml
  label: FirstPromoter Admin API
  slug: firstpromoter-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firstpromoter/refs/heads/main/openapi/firstpromoter-firstpromoter-admin-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Firstpromoter Authentication
name_suffix: Authentication
oauth_flows: []
overview: FirstPromoter secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FirstPromoter
provider_slug: firstpromoter
scheme_count: 1
schemes:
- description: API key passed as Bearer token
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/firstpromoter-firstpromoter-admin-api-openapi.yml
  type: http
slug: firstpromoter-authentication
source_filename: firstpromoter-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/firstpromoter-firstpromoter-admin-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: API key passed as Bearer token\n  sources:\n  - openapi/firstpromoter-firstpromoter-admin-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firstpromoter/refs/heads/main/authentication/firstpromoter-authentication.yml
summary_line: http · 1 scheme
tags:
- Affiliate Marketing
- Referral Tracking
- SaaS
- Commission Management
- Reward Distribution
- Promoters
---
