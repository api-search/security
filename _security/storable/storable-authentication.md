---
api_key_in: []
api_specs:
- filename: storable-openapi.yml
  format: yaml
  label: Storable Tenants API
  slug: storable-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/openapi/storable-openapi.yml
- filename: storable-openapi.yml
  format: yaml
  label: Storable Units & Rate Management API
  slug: storable-units-rate-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/openapi/storable-openapi.yml
- filename: storable-openapi.yml
  format: yaml
  label: Storable Ledgers & Payments API
  slug: storable-ledgers-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/openapi/storable-openapi.yml
- filename: storable-openapi.yml
  format: yaml
  label: Storable Leads & Reservations API
  slug: storable-leads-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/openapi/storable-openapi.yml
- filename: storable-openapi.yml
  format: yaml
  label: Storable Move Ins & Move Outs API
  slug: storable-move-ins-move-outs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/openapi/storable-openapi.yml
- filename: storable-openapi.yml
  format: yaml
  label: Storable Gate Access API
  slug: storable-gate-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/openapi/storable-openapi.yml
- filename: storable-openapi.yml
  format: yaml
  label: Storable Insurance API
  slug: storable-insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/openapi/storable-openapi.yml
- filename: storable-openapi.yml
  format: yaml
  label: Storable Tasks API
  slug: storable-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/openapi/storable-openapi.yml
- filename: storable-openapi.yml
  format: yaml
  label: Storable Documents & eSign API
  slug: storable-documents-esign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/openapi/storable-openapi.yml
- filename: storable-openapi.yml
  format: yaml
  label: Storable Delinquency & Auctions API
  slug: storable-delinquency-auctions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/openapi/storable-openapi.yml
- filename: storable-openapi.yml
  format: yaml
  label: Storable Reporting API
  slug: storable-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/openapi/storable-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Storable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Storable secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Storable
provider_slug: storable
scheme_count: 1
schemes:
- description: 'Non-standard OpenAPI representation of storEDGE''s actual scheme: one-legged OAuth 1.0. The API access key issued to a storEDGE customer is used as the OAuth consumer key and the API secret key as the consumer secret, signing each request; there is no three-legged redirect/token exchange.'
  name: oauth1
  scheme: oauth1
  sources:
  - openapi/storable-openapi.yml
  type: http
slug: storable-authentication
source_filename: storable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/storable-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: oauth1\n  type: http\n  scheme: oauth1\n  description: 'Non-standard OpenAPI representation of storEDGE''s actual scheme: one-legged\n    OAuth 1.0. The API access key issued to a storEDGE customer is used as the OAuth consumer\n    key and the API secret key as the consumer secret, signing each request; there is no three-legged\n    redirect/token exchange.'\n  sources:\n  - openapi/storable-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/authentication/storable-authentication.yml
summary_line: http · 1 scheme
tags:
- Self Storage
- Property Management
- Facility Management
- Tenants
- Reservations
- Payments
- SiteLink
- storEDGE
- SpareFoot
---
