---
api_key_in: []
api_specs:
- filename: uber-codes-api-openapi.yml
  format: yaml
  label: Uber Codes API
  slug: uber-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-codes-api-openapi.yml
- filename: uber-deliveries-api-openapi.yml
  format: yaml
  label: Uber Deliveries API
  slug: uber-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-deliveries-api-openapi.yml
- filename: uber-estimates-api-openapi.yml
  format: yaml
  label: Uber Estimates API
  slug: uber-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-estimates-api-openapi.yml
- filename: uber-locations-api-openapi.yml
  format: yaml
  label: Uber Locations API
  slug: uber-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-locations-api-openapi.yml
- filename: uber-menus-api-openapi.yml
  format: yaml
  label: Uber Menus API
  slug: uber-menus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-menus-api-openapi.yml
- filename: uber-orders-api-openapi.yml
  format: yaml
  label: Uber Orders API
  slug: uber-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-orders-api-openapi.yml
- filename: uber-organizations-api-openapi.yml
  format: yaml
  label: Uber Organizations API
  slug: uber-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-organizations-api-openapi.yml
- filename: uber-partners-api-openapi.yml
  format: yaml
  label: Uber Partners API
  slug: uber-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-partners-api-openapi.yml
- filename: uber-places-api-openapi.yml
  format: yaml
  label: Uber Places API
  slug: uber-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-places-api-openapi.yml
- filename: uber-products-api-openapi.yml
  format: yaml
  label: Uber Products API
  slug: uber-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-products-api-openapi.yml
- filename: uber-programs-api-openapi.yml
  format: yaml
  label: Uber Programs API
  slug: uber-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-programs-api-openapi.yml
- filename: uber-redemption-api-openapi.yml
  format: yaml
  label: Uber Redemption API
  slug: uber-redemption-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-redemption-api-openapi.yml
- filename: uber-refunds-api-openapi.yml
  format: yaml
  label: Uber Refunds API
  slug: uber-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-refunds-api-openapi.yml
- filename: uber-reporting-api-openapi.yml
  format: yaml
  label: Uber Reporting API
  slug: uber-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-reporting-api-openapi.yml
- filename: uber-requests-api-openapi.yml
  format: yaml
  label: Uber Requests API
  slug: uber-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-requests-api-openapi.yml
- filename: uber-riders-api-openapi.yml
  format: yaml
  label: Uber Riders API
  slug: uber-riders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-riders-api-openapi.yml
- filename: uber-stores-api-openapi.yml
  format: yaml
  label: Uber Stores API
  slug: uber-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-stores-api-openapi.yml
- filename: uber-templates-api-openapi.yml
  format: yaml
  label: Uber Templates API
  slug: uber-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-templates-api-openapi.yml
- filename: uber-trips-api-openapi.yml
  format: yaml
  label: Uber Trips API
  slug: uber-trips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-trips-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Uber Authentication
name_suffix: Authentication
oauth_flows: []
overview: Uber secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Uber
provider_slug: uber
scheme_count: 1
schemes:
- description: OAuth 2.0 Bearer token with business.receipts scope
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/uber-businesses-openapi.yml
  - openapi/uber-direct-openapi.yml
  - openapi/uber-drivers-openapi.yml
  - openapi/uber-eats-openapi.yml
  - openapi/uber-riders-openapi.yml
  - openapi/uber-vouchers-openapi.yml
  type: http
slug: uber-authentication
source_filename: uber-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/uber-businesses-openapi.yml, openapi/uber-direct-openapi.yml, openapi/uber-drivers-openapi.yml,\n  openapi/uber-eats-openapi.yml, openapi/uber-riders-openapi.yml, openapi/uber-vouchers-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 Bearer token with business.receipts scope\n  sources:\n  - openapi/uber-businesses-openapi.yml\n  - openapi/uber-direct-openapi.yml\n  - openapi/uber-drivers-openapi.yml\n  - openapi/uber-eats-openapi.yml\n  - openapi/uber-riders-openapi.yml\n  - openapi/uber-vouchers-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/authentication/uber-authentication.yml
summary_line: http · 1 scheme
tags:
- Ridesharing
- Rides
- Taxis
- Transportation
- Food Delivery
- Delivery
- Logistics
---
