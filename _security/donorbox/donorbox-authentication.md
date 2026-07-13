---
api_key_in: []
api_specs:
- filename: donorbox-openapi.yml
  format: yaml
  label: Donorbox Campaigns API
  slug: donorbox-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/donorbox/refs/heads/main/openapi/donorbox-openapi.yml
- filename: donorbox-openapi.yml
  format: yaml
  label: Donorbox Donations API
  slug: donorbox-donations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/donorbox/refs/heads/main/openapi/donorbox-openapi.yml
- filename: donorbox-openapi.yml
  format: yaml
  label: Donorbox Plans API
  slug: donorbox-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/donorbox/refs/heads/main/openapi/donorbox-openapi.yml
- filename: donorbox-openapi.yml
  format: yaml
  label: Donorbox Donors API
  slug: donorbox-donors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/donorbox/refs/heads/main/openapi/donorbox-openapi.yml
- filename: donorbox-openapi.yml
  format: yaml
  label: Donorbox Events API
  slug: donorbox-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/donorbox/refs/heads/main/openapi/donorbox-openapi.yml
- filename: donorbox-openapi.yml
  format: yaml
  label: Donorbox Tickets API
  slug: donorbox-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/donorbox/refs/heads/main/openapi/donorbox-openapi.yml
- filename: donorbox-openapi.yml
  format: yaml
  label: Donorbox Event Ticket Purchases API
  slug: donorbox-purchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/donorbox/refs/heads/main/openapi/donorbox-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Donorbox Authentication
name_suffix: Authentication
oauth_flows: []
overview: Donorbox secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Donorbox
provider_slug: donorbox
scheme_count: 1
schemes:
- description: Username is the Donorbox organization login email; password is the API key generated under Account > API & Zapier Integration.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/donorbox-openapi.yml
  type: http
slug: donorbox-authentication
source_filename: donorbox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/donorbox-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Username is the Donorbox organization login email; password is the API key generated\n    under Account > API & Zapier Integration.\n  sources:\n  - openapi/donorbox-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/donorbox/refs/heads/main/authentication/donorbox-authentication.yml
summary_line: http · 1 scheme
tags:
- Nonprofit
- Fundraising
- Donations
- Payments
- Recurring Giving
- Event Ticketing
---
