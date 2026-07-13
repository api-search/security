---
api_key_in: []
api_specs:
- filename: uber-riders-openapi.yml
  format: yaml
  label: Uber Riders API
  slug: uber-riders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-riders-openapi.yml
- filename: uber-drivers-openapi.yml
  format: yaml
  label: Uber Drivers API
  slug: uber-drivers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-drivers-openapi.yml
- filename: uber-eats-openapi.yml
  format: yaml
  label: Uber Eats API
  slug: uber-eats
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-eats-openapi.yml
- filename: uber-direct-openapi.yml
  format: yaml
  label: Uber Direct API
  slug: uber-direct
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-direct-openapi.yml
- filename: uber-vouchers-openapi.yml
  format: yaml
  label: Uber Vouchers API
  slug: uber-vouchers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-vouchers-openapi.yml
- filename: uber-businesses-openapi.yml
  format: yaml
  label: Uber for Business API
  slug: uber-businesses
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-businesses-openapi.yml
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
- Ride-Sharing
- Rides
- Taxis
- Transportation
- Food Delivery
- Delivery
- Logistics
---
