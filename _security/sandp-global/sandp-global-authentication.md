---
api_key_in: []
api_specs:
- filename: sandp-global-authentication-api-openapi.yml
  format: yaml
  label: S&P Global Authentication API
  slug: sandp-global-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sandp-global/refs/heads/main/openapi/sandp-global-authentication-api-openapi.yml
- filename: sandp-global-financial-data-api-openapi.yml
  format: yaml
  label: S&P Global Financial Data API
  slug: sandp-global-financial-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sandp-global/refs/heads/main/openapi/sandp-global-financial-data-api-openapi.yml
- filename: sandp-global-market-data-api-openapi.yml
  format: yaml
  label: S&P Global Market Data API
  slug: sandp-global-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sandp-global/refs/heads/main/openapi/sandp-global-market-data-api-openapi.yml
- filename: sandp-global-price-assessments-api-openapi.yml
  format: yaml
  label: S&P Global Price Assessments API
  slug: sandp-global-price-assessments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sandp-global/refs/heads/main/openapi/sandp-global-price-assessments-api-openapi.yml
- filename: sandp-global-reference-data-api-openapi.yml
  format: yaml
  label: S&P Global Reference Data API
  slug: sandp-global-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sandp-global/refs/heads/main/openapi/sandp-global-reference-data-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sandp Global Authentication
name_suffix: Authentication
oauth_flows: []
overview: S&P Global secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: S&P Global
provider_slug: sandp-global
scheme_count: 1
schemes:
- description: Bearer token obtained from the /authenticate/api/v1/token endpoint
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/sandp-global-capital-iq-openapi.yml
  - openapi/sandp-global-commodity-insights-openapi.yml
  type: http
slug: sandp-global-authentication
source_filename: sandp-global-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sandp-global-capital-iq-openapi.yml, openapi/sandp-global-commodity-insights-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token obtained from the /authenticate/api/v1/token endpoint\n  sources:\n  - openapi/sandp-global-capital-iq-openapi.yml\n  - openapi/sandp-global-commodity-insights-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sandp-global/refs/heads/main/authentication/sandp-global-authentication.yml
summary_line: http · 1 scheme
tags:
- Financial Data
- Market Intelligence
- Commodity Insights
- Credit Ratings
- Analytics
- Fortune 500
- Enterprise
---
