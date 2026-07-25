---
api_key_in:
- header
api_specs:
- filename: tapfiliate-affiliate-groups-api-openapi.yml
  format: yaml
  label: Tapfiliate Affiliate Groups API
  slug: tapfiliate-affiliate-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/openapi/tapfiliate-affiliate-groups-api-openapi.yml
- filename: tapfiliate-affiliate-prospects-api-openapi.yml
  format: yaml
  label: Tapfiliate Affiliate Prospects API
  slug: tapfiliate-affiliate-prospects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/openapi/tapfiliate-affiliate-prospects-api-openapi.yml
- filename: tapfiliate-affiliates-api-openapi.yml
  format: yaml
  label: Tapfiliate Affiliates API
  slug: tapfiliate-affiliates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/openapi/tapfiliate-affiliates-api-openapi.yml
- filename: tapfiliate-balances-api-openapi.yml
  format: yaml
  label: Tapfiliate Balances API
  slug: tapfiliate-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/openapi/tapfiliate-balances-api-openapi.yml
- filename: tapfiliate-clicks-api-openapi.yml
  format: yaml
  label: Tapfiliate Clicks API
  slug: tapfiliate-clicks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/openapi/tapfiliate-clicks-api-openapi.yml
- filename: tapfiliate-commissions-api-openapi.yml
  format: yaml
  label: Tapfiliate Commissions API
  slug: tapfiliate-commissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/openapi/tapfiliate-commissions-api-openapi.yml
- filename: tapfiliate-conversions-api-openapi.yml
  format: yaml
  label: Tapfiliate Conversions API
  slug: tapfiliate-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/openapi/tapfiliate-conversions-api-openapi.yml
- filename: tapfiliate-customers-api-openapi.yml
  format: yaml
  label: Tapfiliate Customers API
  slug: tapfiliate-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/openapi/tapfiliate-customers-api-openapi.yml
- filename: tapfiliate-payments-api-openapi.yml
  format: yaml
  label: Tapfiliate Payments API
  slug: tapfiliate-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/openapi/tapfiliate-payments-api-openapi.yml
- filename: tapfiliate-programs-api-openapi.yml
  format: yaml
  label: Tapfiliate Programs API
  slug: tapfiliate-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/openapi/tapfiliate-programs-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tapfiliate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tapfiliate secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tapfiliate
provider_slug: tapfiliate
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/tapfiliate-rest-api-openapi.yml
  type: apiKey
slug: tapfiliate-authentication
source_filename: tapfiliate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tapfiliate-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/tapfiliate-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/authentication/tapfiliate-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Affiliate Marketing
- Affiliate Tracking
- Commission Management
- Conversion Tracking
- Partner Programs
- Referral Programs
- Influencer Marketing
---
