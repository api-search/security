---
api_key_in: []
api_specs:
- filename: servicecatalog
  format: yaml
  label: S&P Global Commodity Insights API
  slug: commodity-insights
  spec_type: OpenAPI
  url: https://developer.spglobal.com/commodityinsights/servicecatalog
- filename: s-and-p-global-kensho-link-openapi.yml
  format: yaml
  label: Kensho Link API
  slug: kensho-link
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s-and-p-global/refs/heads/main/openapi/s-and-p-global-kensho-link-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: S And P Global Authentication
name_suffix: Authentication
oauth_flows: []
overview: S&P Global secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: S&P Global
provider_slug: s-and-p-global
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/s-and-p-global-commodity-insights-openapi.yml
  - openapi/s-and-p-global-kensho-link-openapi.yml
  type: http
slug: s-and-p-global-authentication
source_filename: s-and-p-global-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/s-and-p-global-commodity-insights-openapi.yml, openapi/s-and-p-global-kensho-link-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/s-and-p-global-commodity-insights-openapi.yml\n  - openapi/s-and-p-global-kensho-link-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/s-and-p-global/refs/heads/main/authentication/s-and-p-global-authentication.yml
summary_line: http · 1 scheme
tags:
- Financial Data
- Credit Ratings
- Market Intelligence
- Commodity Insights
- Energy Markets
- Capital Markets
- Fortune 500
---
