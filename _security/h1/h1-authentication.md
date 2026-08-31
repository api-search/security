---
api_key_in: []
api_specs:
- filename: h1-cost-estimates-api-openapi.yml
  format: yaml
  label: H1 Cost Estimates API
  slug: h1-insights-cost-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1/refs/heads/main/openapi/h1-cost-estimates-api-openapi.yml
- filename: h1-filters-api-openapi.yml
  format: yaml
  label: H1 Filters API
  slug: h1-insights-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1/refs/heads/main/openapi/h1-filters-api-openapi.yml
- filename: h1-focus-area-endpoints-api-openapi.yml
  format: yaml
  label: H1 Focus Area Endpoints API
  slug: h1-insights-focus-area-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1/refs/heads/main/openapi/h1-focus-area-endpoints-api-openapi.yml
- filename: h1-locations-api-openapi.yml
  format: yaml
  label: H1 Locations API
  slug: h1-insights-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1/refs/heads/main/openapi/h1-locations-api-openapi.yml
- filename: h1-networks-api-openapi.yml
  format: yaml
  label: H1 Networks API
  slug: h1-insights-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1/refs/heads/main/openapi/h1-networks-api-openapi.yml
- filename: h1-organizations-api-openapi.yml
  format: yaml
  label: H1 Organizations API
  slug: h1-insights-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1/refs/heads/main/openapi/h1-organizations-api-openapi.yml
- filename: h1-price-transparency-api-openapi.yml
  format: yaml
  label: H1 Price Transparency API
  slug: h1-insights-price-transparency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1/refs/heads/main/openapi/h1-price-transparency-api-openapi.yml
- filename: h1-providers-api-openapi.yml
  format: yaml
  label: H1 Providers API
  slug: h1-insights-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1/refs/heads/main/openapi/h1-providers-api-openapi.yml
- filename: h1-reference-endpoints-api-openapi.yml
  format: yaml
  label: H1 Reference Endpoints API
  slug: h1-insights-reference-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1/refs/heads/main/openapi/h1-reference-endpoints-api-openapi.yml
- filename: h1-tins-api-openapi.yml
  format: yaml
  label: H1 TI Ns API
  slug: h1-insights-tins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1/refs/heads/main/openapi/h1-tins-api-openapi.yml
- filename: h1-virtual-care-platforms-api-openapi.yml
  format: yaml
  label: H1 Virtual Care Platforms API
  slug: h1-insights-virtual-care-platforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1/refs/heads/main/openapi/h1-virtual-care-platforms-api-openapi.yml
- filename: h1-price-transparency-v2-api-openapi.yml
  format: yaml
  label: H1 Price Transparency v2 API
  slug: h1-price-transparency-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1/refs/heads/main/openapi/h1-price-transparency-v2-api-openapi.yml
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
- applied: global
  format: Bearer {customer_token}
  header: Authorization
  in: header
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/ribbon-health-api-openapi.json
  - openapi/h1-price-transparency-v2-openapi.json
  type: http
slug: h1-authentication
source_filename: h1-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: searched\nsource: openapi/ribbon-health-api-openapi.json, openapi/h1-price-transparency-v2-openapi.json\ndocs: https://ribbon.readme.io/docs/authentication\nsummary:\n  types:\n  - http\n  scheme: bearer-api-key\n  key_prefix: null\n  note: >-\n    The H1 (Ribbon Health) API authenticates every request with a customer API\n    key passed in the HTTP Bearer scheme - Authorization: Bearer {customer_token}.\n    Both published contracts - the v1 API and Price Transparency v2 - declare the\n    same single BearerAuth scheme and apply it globally. There is no OAuth 2.0 /\n    OpenID Connect surface (no /.well-known/oauth-authorization-server or\n    openid-configuration on any host, probed 2026-08-15), so there are no scopes\n    and no scopes/ artifact. Authorization is expressed instead as per-account\n    entitlement flags such as `doctors.can_price_transparency`, which surface as a\n    403 rather than as a scope check. Keys are issued via the\
  \ request-demo\n    onboarding rather than self-serve. No published key prefix or format. Keep the\n    key server-side; H1's docs explicitly warn against client-side use.\nauthorization:\n  model: account-entitlement-flags\n  scopes: []\n  observed_flags:\n  - doctors.can_price_transparency\n  failure_status: 403\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: Bearer {customer_token}\n  applied: global\n  sources:\n  - openapi/ribbon-health-api-openapi.json\n  - openapi/h1-price-transparency-v2-openapi.json\n"
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
