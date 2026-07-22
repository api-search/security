---
api_key_in: []
api_specs:
- filename: uncapped-partners-openapi-original.json
  format: json
  label: Uncapped Partners API
  slug: uncapped-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uncapped/refs/heads/main/openapi/uncapped-partners-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Uncapped Authentication
name_suffix: Authentication
oauth_flows: []
overview: Uncapped secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Uncapped
provider_slug: uncapped
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: auth0_bearer
  scheme: bearer
  sources:
  - openapi/uncapped-partners-openapi-original.json
  type: http
slug: uncapped-authentication
source_filename: uncapped-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/uncapped-partners-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: auth0_bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/uncapped-partners-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uncapped/refs/heads/main/authentication/uncapped-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fintech
- Lending
- Embedded Finance
- Revenue-Based Financing
- Working Capital
- eCommerce
---
