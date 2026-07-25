---
api_key_in: []
api_specs:
- filename: ribbon-health-api-openapi.json
  format: json
  label: H1 Ribbon Providers API
  slug: ribbon-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1/refs/heads/main/openapi/ribbon-health-api-openapi.json
- filename: ribbon-health-api-openapi.json
  format: json
  label: H1 Ribbon Locations API
  slug: ribbon-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1/refs/heads/main/openapi/ribbon-health-api-openapi.json
- filename: ribbon-health-api-openapi.json
  format: json
  label: H1 Ribbon Custom Filters API
  slug: ribbon-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1/refs/heads/main/openapi/ribbon-health-api-openapi.json
- filename: ribbon-health-api-openapi.json
  format: json
  label: H1 Ribbon Focus Areas API
  slug: ribbon-focus-areas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1/refs/heads/main/openapi/ribbon-health-api-openapi.json
- filename: ribbon-health-api-openapi.json
  format: json
  label: H1 Ribbon Price Transparency API
  slug: ribbon-price-transparency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1/refs/heads/main/openapi/ribbon-health-api-openapi.json
- filename: ribbon-health-api-openapi.json
  format: json
  label: H1 Ribbon Cost Estimates & Eligibility API
  slug: ribbon-cost-estimates-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1/refs/heads/main/openapi/ribbon-health-api-openapi.json
- filename: ribbon-health-api-openapi.json
  format: json
  label: H1 Ribbon Organizations API
  slug: ribbon-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1/refs/heads/main/openapi/ribbon-health-api-openapi.json
- filename: ribbon-health-api-openapi.json
  format: json
  label: H1 Ribbon Reference Data API
  slug: ribbon-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1/refs/heads/main/openapi/ribbon-health-api-openapi.json
- filename: ribbon-health-api-openapi.json
  format: json
  label: H1 Ribbon Network Analysis API
  slug: ribbon-network-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1/refs/heads/main/openapi/ribbon-health-api-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: H1 Authentication
name_suffix: Authentication
oauth_flows: []
overview: H1 secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: H1
provider_slug: h1
scheme_count: 1
schemes:
- format: Bearer {customer_token}
  header: Authorization
  in: header
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/ribbon-health-api-openapi.json
  type: http
slug: h1-authentication
source_filename: h1-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: openapi/ribbon-health-api-openapi.json\ndocs: https://ribbon.readme.io/docs/authentication\nsummary:\n  types:\n  - http\n  scheme: bearer-api-key\n  note: >-\n    The H1 (Ribbon Health) API authenticates every request with a customer API\n    key passed in the HTTP Bearer scheme - Authorization: Bearer {customer_token}.\n    There is no OAuth 2.0 / OpenID Connect surface; keys are issued via the\n    request-demo onboarding rather than self-serve. Keep the key server-side.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: Bearer {customer_token}\n  sources:\n  - openapi/ribbon-health-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/h1/refs/heads/main/authentication/h1-authentication.yml
summary_line: http · 1 scheme
tags:
- Healthcare
- United States
- Life Sciences
- Provider Data
- Healthcare API
- Price Transparency
- Eligibility
- Network Intelligence
- Digital Health
- Pharma
---
