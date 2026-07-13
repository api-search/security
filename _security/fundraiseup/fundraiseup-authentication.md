---
api_key_in: []
api_specs:
- filename: fundraiseup-openapi.yml
  format: yaml
  label: Fundraise Up Donations API
  slug: fundraiseup-donations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundraiseup/refs/heads/main/openapi/fundraiseup-openapi.yml
- filename: fundraiseup-openapi.yml
  format: yaml
  label: Fundraise Up Recurring Plans API
  slug: fundraiseup-recurring-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundraiseup/refs/heads/main/openapi/fundraiseup-openapi.yml
- filename: fundraiseup-openapi.yml
  format: yaml
  label: Fundraise Up Supporters API
  slug: fundraiseup-supporters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundraiseup/refs/heads/main/openapi/fundraiseup-openapi.yml
- filename: fundraiseup-openapi.yml
  format: yaml
  label: Fundraise Up Events API
  slug: fundraiseup-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundraiseup/refs/heads/main/openapi/fundraiseup-openapi.yml
- filename: fundraiseup-openapi.yml
  format: yaml
  label: Fundraise Up Donor Portal Access Links API
  slug: fundraiseup-donor-portal-access-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundraiseup/refs/heads/main/openapi/fundraiseup-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
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
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fundraiseup/refs/heads/main/authentication/fundraiseup-authentication.yml
summary_line: http · 1 scheme
tags:
- Fundraising
- Donations
- Nonprofit
- Payments
- Recurring Giving
- Donor Management
---
