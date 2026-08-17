---
api_key_in: []
api_specs:
- filename: fund-that-flip-flipperforce-public-api.yml
  format: yaml
  label: FlipperForce Public API
  slug: flipperforce-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fund-that-flip/refs/heads/main/openapi/fund-that-flip-flipperforce-public-api.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fund That Flip Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fund That Flip secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fund That Flip
provider_slug: fund-that-flip
scheme_count: 1
schemes:
- bearerFormat: FlipperForce Public API key
  description: 'Use the Public API key provided by FlipperForce as a Bearer token. Send the key exactly as provided in the Authorization header: `Authorization: Bearer <api-key>`.'
  name: PublicApiBearerAuth
  scheme: bearer
  sources:
  - openapi/fund-that-flip-flipperforce-public-api.yml
  type: http
slug: fund-that-flip-authentication
source_filename: fund-that-flip-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: derived\nsource: openapi/fund-that-flip-flipperforce-public-api.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: PublicApiBearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: FlipperForce Public API key\n  description: 'Use the Public API key provided by FlipperForce as a Bearer token. Send the\n    key exactly as provided in the Authorization header: `Authorization: Bearer <api-key>`.'\n  sources:\n  - openapi/fund-that-flip-flipperforce-public-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fund-that-flip/refs/heads/main/authentication/fund-that-flip-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Real Estate
- Lending
- Construction
- Project Management
- Financial Services
- Investing
- Fintech
- Property Technology
- Accounting
---
