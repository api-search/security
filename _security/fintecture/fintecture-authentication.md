---
api_key_in: []
api_specs:
- filename: fintecture-pis-api-openapi.yml
  format: yaml
  label: Fintecture Payment Initiation Services API
  slug: fintecture-pis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintecture/refs/heads/main/openapi/fintecture-pis-api-openapi.yml
- filename: fintecture-ais-api-openapi.yml
  format: yaml
  label: Fintecture Account Information Services API
  slug: fintecture-ais-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintecture/refs/heads/main/openapi/fintecture-ais-api-openapi.yml
- filename: fintecture-customers-api-openapi.yml
  format: yaml
  label: Fintecture Customers API
  slug: fintecture-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintecture/refs/heads/main/openapi/fintecture-customers-api-openapi.yml
- filename: fintecture-emandates-api-openapi.yml
  format: yaml
  label: Fintecture E-Mandates API
  slug: fintecture-emandates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintecture/refs/heads/main/openapi/fintecture-emandates-api-openapi.yml
- filename: fintecture-oauth-api-openapi.yml
  format: yaml
  label: Fintecture OAuth and Tokens API
  slug: fintecture-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintecture/refs/heads/main/openapi/fintecture-oauth-api-openapi.yml
- filename: fintecture-resources-api-openapi.yml
  format: yaml
  label: Fintecture Resources API
  slug: fintecture-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintecture/refs/heads/main/openapi/fintecture-resources-api-openapi.yml
- filename: fintecture-oac-api-openapi.yml
  format: yaml
  label: Fintecture Organisation Access Credentials API
  slug: fintecture-oac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintecture/refs/heads/main/openapi/fintecture-oac-api-openapi.yml
- filename: fintecture-transactions-api-openapi.yml
  format: yaml
  label: Fintecture Transactions and Settlements API
  slug: fintecture-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintecture/refs/heads/main/openapi/fintecture-transactions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fintecture Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fintecture secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fintecture
provider_slug: fintecture
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/fintecture-ais-api-openapi.yml
  - openapi/fintecture-customers-api-openapi.yml
  - openapi/fintecture-emandates-api-openapi.yml
  - openapi/fintecture-oac-api-openapi.yml
  - openapi/fintecture-pis-api-openapi.yml
  - openapi/fintecture-resources-api-openapi.yml
  - openapi/fintecture-transactions-api-openapi.yml
  type: http
slug: fintecture-authentication
source_filename: fintecture-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fintecture-ais-api-openapi.yml, openapi/fintecture-customers-api-openapi.yml,\n  openapi/fintecture-emandates-api-openapi.yml, openapi/fintecture-oac-api-openapi.yml, openapi/fintecture-pis-api-openapi.yml,\n  openapi/fintecture-resources-api-openapi.yml, openapi/fintecture-transactions-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/fintecture-ais-api-openapi.yml\n  - openapi/fintecture-customers-api-openapi.yml\n  - openapi/fintecture-emandates-api-openapi.yml\n  - openapi/fintecture-oac-api-openapi.yml\n  - openapi/fintecture-pis-api-openapi.yml\n  - openapi/fintecture-resources-api-openapi.yml\n  - openapi/fintecture-transactions-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fintecture/refs/heads/main/authentication/fintecture-authentication.yml
summary_line: http · 1 scheme
tags:
- Open Banking
- Payments
- PSD2
- France
- Account Information
- Payment Initiation
- Instant Payments
- SEPA
- Smart Transfer
- Request To Pay
- Buy Now Pay Later
- E-Mandates
- Account-to-Account
- KYC
---
