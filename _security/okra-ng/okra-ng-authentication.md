---
api_key_in: []
api_specs:
- filename: okra-ng-openapi.yml
  format: yaml
  label: Okra Auth & Link API
  slug: okra-ng-auth-link-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-ng/refs/heads/main/openapi/okra-ng-openapi.yml
- filename: okra-ng-openapi.yml
  format: yaml
  label: Okra Accounts & Balance API
  slug: okra-ng-accounts-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-ng/refs/heads/main/openapi/okra-ng-openapi.yml
- filename: okra-ng-openapi.yml
  format: yaml
  label: Okra Transactions API
  slug: okra-ng-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-ng/refs/heads/main/openapi/okra-ng-openapi.yml
- filename: okra-ng-openapi.yml
  format: yaml
  label: Okra Identity & Income API
  slug: okra-ng-identity-income-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-ng/refs/heads/main/openapi/okra-ng-openapi.yml
- filename: okra-ng-openapi.yml
  format: yaml
  label: Okra Payments API
  slug: okra-ng-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-ng/refs/heads/main/openapi/okra-ng-openapi.yml
- filename: okra-ng-openapi.yml
  format: yaml
  label: Okra Webhooks API
  slug: okra-ng-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-ng/refs/heads/main/openapi/okra-ng-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Okra Ng Authentication
name_suffix: Authentication
oauth_flows: []
overview: Okra secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Okra
provider_slug: okra-ng
scheme_count: 1
schemes:
- description: Okra secret API key supplied as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/okra-ng-openapi.yml
  type: http
slug: okra-ng-authentication
source_filename: okra-ng-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/okra-ng-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Okra secret API key supplied as a Bearer token.\n  sources:\n  - openapi/okra-ng-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/okra-ng/refs/heads/main/authentication/okra-ng-authentication.yml
summary_line: http · 1 scheme
tags:
- Open Banking
- Open Finance
- Fintech
- Africa
- Nigeria
- Financial Data
---
