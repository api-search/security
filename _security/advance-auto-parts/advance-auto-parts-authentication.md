---
api_key_in:
- header
api_specs:
- filename: advance-auto-parts-catalog-api-openapi.yml
  format: yaml
  label: Advance Auto Parts Catalog API
  slug: advance-auto-parts-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advance-auto-parts/refs/heads/main/openapi/advance-auto-parts-catalog-api-openapi.yml
- filename: advance-auto-parts-commerce-api-openapi.yml
  format: yaml
  label: Advance Auto Parts Commerce API
  slug: advance-auto-parts-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advance-auto-parts/refs/heads/main/openapi/advance-auto-parts-commerce-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Advance Auto Parts Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Advance Auto Parts secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Advance Auto Parts
provider_slug: advance-auto-parts
scheme_count: 2
schemes:
- in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/advance-auto-parts-catalog-api-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://auth.advanceautoparts.com/oauth/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://auth.advanceautoparts.com/oauth/token
  name: oauth2
  sources:
  - openapi/advance-auto-parts-commerce-api-openapi.yml
  type: oauth2
slug: advance-auto-parts-authentication
source_filename: advance-auto-parts-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/advance-auto-parts-catalog-api-openapi.yml, openapi/advance-auto-parts-commerce-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/advance-auto-parts-catalog-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.advanceautoparts.com/oauth/authorize\n    tokenUrl: https://auth.advanceautoparts.com/oauth/token\n    scopes: 4\n  sources:\n  - openapi/advance-auto-parts-commerce-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advance-auto-parts/refs/heads/main/authentication/advance-auto-parts-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Automotive
- E-Commerce
- Parts Catalog
- Retail
- Supply Chain
- Fortune 500
---
