---
api_key_in: []
api_specs:
- filename: givebutter-campaigns-api-openapi.yml
  format: yaml
  label: Givebutter Campaigns API
  slug: givebutter-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/givebutter/refs/heads/main/openapi/givebutter-campaigns-api-openapi.yml
- filename: givebutter-contacts-api-openapi.yml
  format: yaml
  label: Givebutter Contacts API
  slug: givebutter-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/givebutter/refs/heads/main/openapi/givebutter-contacts-api-openapi.yml
- filename: givebutter-discount-codes-api-openapi.yml
  format: yaml
  label: Givebutter Discount Codes API
  slug: givebutter-discount-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/givebutter/refs/heads/main/openapi/givebutter-discount-codes-api-openapi.yml
- filename: givebutter-funds-api-openapi.yml
  format: yaml
  label: Givebutter Funds API
  slug: givebutter-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/givebutter/refs/heads/main/openapi/givebutter-funds-api-openapi.yml
- filename: givebutter-payouts-api-openapi.yml
  format: yaml
  label: Givebutter Payouts API
  slug: givebutter-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/givebutter/refs/heads/main/openapi/givebutter-payouts-api-openapi.yml
- filename: givebutter-plans-api-openapi.yml
  format: yaml
  label: Givebutter Plans API
  slug: givebutter-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/givebutter/refs/heads/main/openapi/givebutter-plans-api-openapi.yml
- filename: givebutter-tickets-api-openapi.yml
  format: yaml
  label: Givebutter Tickets API
  slug: givebutter-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/givebutter/refs/heads/main/openapi/givebutter-tickets-api-openapi.yml
- filename: givebutter-transactions-api-openapi.yml
  format: yaml
  label: Givebutter Transactions API
  slug: givebutter-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/givebutter/refs/heads/main/openapi/givebutter-transactions-api-openapi.yml
- filename: givebutter-webhooks-api-openapi.yml
  format: yaml
  label: Givebutter Webhooks API
  slug: givebutter-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/givebutter/refs/heads/main/openapi/givebutter-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Givebutter Authentication
name_suffix: Authentication
oauth_flows: []
overview: Givebutter secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Givebutter
provider_slug: givebutter
scheme_count: 1
schemes:
- bearerFormat: API Key
  description: Bearer token authentication using a personal API key.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/givebutter-openapi.yml
  type: http
slug: givebutter-authentication
source_filename: givebutter-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/givebutter-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: Bearer token authentication using a personal API key.\n  sources:\n  - openapi/givebutter-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/givebutter/refs/heads/main/authentication/givebutter-authentication.yml
summary_line: http · 1 scheme
tags:
- Donations
- Fundraising
- Nonprofits
---
