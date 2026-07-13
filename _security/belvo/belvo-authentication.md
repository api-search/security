---
api_key_in: []
api_specs:
- filename: belvo-openapi.yml
  format: yaml
  label: Belvo Links API
  slug: belvo-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/belvo/refs/heads/main/openapi/belvo-openapi.yml
- filename: belvo-openapi.yml
  format: yaml
  label: Belvo Accounts API
  slug: belvo-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/belvo/refs/heads/main/openapi/belvo-openapi.yml
- filename: belvo-openapi.yml
  format: yaml
  label: Belvo Transactions & Balances API
  slug: belvo-transactions-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/belvo/refs/heads/main/openapi/belvo-openapi.yml
- filename: belvo-openapi.yml
  format: yaml
  label: Belvo Owners & Incomes API
  slug: belvo-owners-incomes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/belvo/refs/heads/main/openapi/belvo-openapi.yml
- filename: belvo-openapi.yml
  format: yaml
  label: Belvo Institutions API
  slug: belvo-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/belvo/refs/heads/main/openapi/belvo-openapi.yml
- filename: belvo-openapi.yml
  format: yaml
  label: Belvo Payments (Brazil / Pix) API
  slug: belvo-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/belvo/refs/heads/main/openapi/belvo-openapi.yml
- filename: belvo-openapi.yml
  format: yaml
  label: Belvo Webhooks API
  slug: belvo-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/belvo/refs/heads/main/openapi/belvo-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Belvo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Belvo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Belvo
provider_slug: belvo
scheme_count: 1
schemes:
- description: HTTP Basic authentication using your Secret Key ID as the username and your Secret Key Password as the password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/belvo-openapi.yml
  type: http
slug: belvo-authentication
source_filename: belvo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/belvo-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using your Secret Key ID as the username and your Secret\n    Key Password as the password.\n  sources:\n  - openapi/belvo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/belvo/refs/heads/main/authentication/belvo-authentication.yml
summary_line: http · 1 scheme
tags:
- Open Finance
- Open Banking
- Bank Data
- Aggregation
- Payments
- Pix
- Latin America
---
