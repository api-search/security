---
api_key_in: []
api_specs:
- filename: good-leap-developer-api-openapi.yml
  format: yaml
  label: GoodLeap Developer API
  slug: goodleap-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/good-leap/refs/heads/main/openapi/good-leap-developer-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Good Leap Authentication
name_suffix: Authentication
oauth_flows: []
overview: Good Leap secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Good Leap
provider_slug: good-leap
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT obtained via POST /posfinancing/rest/v2/auth/token (organizationId), refreshed via /auth/token/refresh.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/good-leap-developer-api-openapi.yml
  type: http
slug: good-leap-authentication
source_filename: good-leap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/good-leap-developer-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT obtained via POST /posfinancing/rest/v2/auth/token (organizationId), refreshed\n    via /auth/token/refresh.\n  sources:\n  - openapi/good-leap-developer-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/good-leap/refs/heads/main/authentication/good-leap-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fintech
- Financing
- Lending
- Solar
- Home Improvement
- Sustainability
- Point of Sale
- Loans
- Payments
---
