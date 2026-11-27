---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mynto-no-bank-api-openapi.yml
  format: yaml
  label: Mynto Bank API
  slug: mynto-no-bank-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mynto-no/openapi/mynto-no-bank-api-openapi.yml
- filename: mynto-no-invoicing-api-openapi.yml
  format: yaml
  label: Mynto Invoicing API
  slug: mynto-no-invoicing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mynto-no/openapi/mynto-no-invoicing-api-openapi.yml
- filename: mynto-no-ledger-api-openapi.yml
  format: yaml
  label: Mynto Ledger API
  slug: mynto-no-ledger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mynto-no/openapi/mynto-no-ledger-api-openapi.yml
- filename: mynto-no-webhooks-api-openapi.yml
  format: yaml
  label: Mynto Webhooks API
  slug: mynto-no-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mynto-no/openapi/mynto-no-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Mynto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mynto secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mynto
provider_slug: mynto-no
scheme_count: 1
schemes:
- description: A personal API key (mynto_sk_…) or an OAuth 2.1 access token (mynto_at_…).
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/mynto-no-openapi.yml
  type: http
slug: mynto-no-authentication
source_filename: mynto-no-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/mynto-no-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: A personal API key (mynto_sk_…) or an OAuth 2.1 access token (mynto_at_…).\n  sources:\n  - openapi/mynto-no-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/mynto-no/authentication/mynto-no-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Accounting
- Automation
- Finance
- Software-as-a-Service
- Norway
---
