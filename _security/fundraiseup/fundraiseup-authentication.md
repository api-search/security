---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fundraiseup-donations-api-openapi.yml
  format: yaml
  label: Fundraise Up Donations API
  slug: fundraiseup-donations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fundraiseup/openapi/fundraiseup-donations-api-openapi.yml
- filename: fundraiseup-events-api-openapi.yml
  format: yaml
  label: Fundraise Up Events API
  slug: fundraiseup-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fundraiseup/openapi/fundraiseup-events-api-openapi.yml
- filename: fundraiseup-recurring-plans-api-openapi.yml
  format: yaml
  label: Fundraise Up Recurring Plans API
  slug: fundraiseup-recurring-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fundraiseup/openapi/fundraiseup-recurring-plans-api-openapi.yml
- filename: fundraiseup-supporters-api-openapi.yml
  format: yaml
  label: Fundraise Up Supporters API
  slug: fundraiseup-supporters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fundraiseup/openapi/fundraiseup-supporters-api-openapi.yml
- filename: fundraiseup-access-links-api-openapi.yml
  format: yaml
  label: Fundraise Up Access links API
  slug: fundraiseup-access-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fundraiseup/openapi/fundraiseup-access-links-api-openapi.yml
- filename: fundraiseup-campaigns-api-openapi.yml
  format: yaml
  label: Fundraise Up Campaigns API
  slug: fundraiseup-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fundraiseup/openapi/fundraiseup-campaigns-api-openapi.yml
- filename: fundraiseup-designation-configurations-api-openapi.yml
  format: yaml
  label: Fundraise Up Designation configurations API
  slug: fundraiseup-designation-configurations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fundraiseup/openapi/fundraiseup-designation-configurations-api-openapi.yml
- filename: fundraiseup-designation-groups-api-openapi.yml
  format: yaml
  label: Fundraise Up Designation groups API
  slug: fundraiseup-designation-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fundraiseup/openapi/fundraiseup-designation-groups-api-openapi.yml
- filename: fundraiseup-designations-api-openapi.yml
  format: yaml
  label: Fundraise Up Designations API
  slug: fundraiseup-designations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fundraiseup/openapi/fundraiseup-designations-api-openapi.yml
- filename: fundraiseup-fundraisers-api-openapi.yml
  format: yaml
  label: Fundraise Up Fundraisers API
  slug: fundraiseup-fundraisers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fundraiseup/openapi/fundraiseup-fundraisers-api-openapi.yml
- filename: fundraiseup-upgrade-links-api-openapi.yml
  format: yaml
  label: Fundraise Up Upgrade links API
  slug: fundraiseup-upgrade-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fundraiseup/openapi/fundraiseup-upgrade-links-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Fundraiseup Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fundraise Up secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fundraise Up
provider_slug: fundraiseup
scheme_count: 1
schemes:
- description: API key created in the dashboard under Settings > API keys, sent as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/fundraiseup-openapi.yml
  type: http
slug: fundraiseup-authentication
source_filename: fundraiseup-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fundraiseup-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key created in the dashboard under Settings > API keys, sent as a Bearer\n    token.\n  sources:\n  - openapi/fundraiseup-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/fundraiseup/authentication/fundraiseup-authentication.yml
summary_line: http · 1 scheme
tags:
- Fundraising
- Donations
- Non-Profit
- Payments
- Recurring Giving
- Donor Management
---
