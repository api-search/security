---
anonymous_access: false
api_key_in: []
api_specs:
- filename: chrome-river-accounts-api-openapi.yml
  format: yaml
  label: Chrome River Accounts API
  slug: chrome-river-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chrome-river/refs/heads/main/openapi/chrome-river-accounts-api-openapi.yml
- filename: chrome-river-allowances-api-openapi.yml
  format: yaml
  label: Chrome River Allowances API
  slug: chrome-river-allowances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chrome-river/refs/heads/main/openapi/chrome-river-allowances-api-openapi.yml
- filename: chrome-river-cards-api-openapi.yml
  format: yaml
  label: Chrome River Cards API
  slug: chrome-river-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chrome-river/refs/heads/main/openapi/chrome-river-cards-api-openapi.yml
- filename: chrome-river-categories-api-openapi.yml
  format: yaml
  label: Chrome River Categories API
  slug: chrome-river-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chrome-river/refs/heads/main/openapi/chrome-river-categories-api-openapi.yml
- filename: chrome-river-company-api-openapi.yml
  format: yaml
  label: Chrome River Company API
  slug: chrome-river-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chrome-river/refs/heads/main/openapi/chrome-river-company-api-openapi.yml
- filename: chrome-river-departments-api-openapi.yml
  format: yaml
  label: Chrome River Departments API
  slug: chrome-river-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chrome-river/refs/heads/main/openapi/chrome-river-departments-api-openapi.yml
- filename: chrome-river-labels-api-openapi.yml
  format: yaml
  label: Chrome River Labels API
  slug: chrome-river-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chrome-river/refs/heads/main/openapi/chrome-river-labels-api-openapi.yml
- filename: chrome-river-locations-api-openapi.yml
  format: yaml
  label: Chrome River Locations API
  slug: chrome-river-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chrome-river/refs/heads/main/openapi/chrome-river-locations-api-openapi.yml
- filename: chrome-river-members-api-openapi.yml
  format: yaml
  label: Chrome River Members API
  slug: chrome-river-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chrome-river/refs/heads/main/openapi/chrome-river-members-api-openapi.yml
- filename: chrome-river-merchant-categories-api-openapi.yml
  format: yaml
  label: Chrome River Merchant Categories API
  slug: chrome-river-merchant-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chrome-river/refs/heads/main/openapi/chrome-river-merchant-categories-api-openapi.yml
- filename: chrome-river-oauth-api-openapi.yml
  format: yaml
  label: Chrome River OAuth API
  slug: chrome-river-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chrome-river/refs/heads/main/openapi/chrome-river-oauth-api-openapi.yml
- filename: chrome-river-requisitions-api-openapi.yml
  format: yaml
  label: Chrome River Requisitions API
  slug: chrome-river-requisitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chrome-river/refs/heads/main/openapi/chrome-river-requisitions-api-openapi.yml
- filename: chrome-river-shared-links-api-openapi.yml
  format: yaml
  label: Chrome River Shared Links API
  slug: chrome-river-shared-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chrome-river/refs/heads/main/openapi/chrome-river-shared-links-api-openapi.yml
- filename: chrome-river-shipping-addresses-api-openapi.yml
  format: yaml
  label: Chrome River Shipping Addresses API
  slug: chrome-river-shipping-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chrome-river/refs/heads/main/openapi/chrome-river-shipping-addresses-api-openapi.yml
- filename: chrome-river-transactions-api-openapi.yml
  format: yaml
  label: Chrome River Transactions API
  slug: chrome-river-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chrome-river/refs/heads/main/openapi/chrome-river-transactions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Chrome River Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chrome River secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Chrome River
provider_slug: chrome-river
scheme_count: 1
schemes:
- description: 'OAuth2 access token. Include in Authorization header: `Authorization: Bearer YOUR_ACCESS_TOKEN`'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/chrome-river-openapi.json
  type: http
slug: chrome-river-authentication
source_filename: chrome-river-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: derived\nsource: openapi/chrome-river-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'OAuth2 access token. Include in Authorization header: `Authorization: Bearer\n    YOUR_ACCESS_TOKEN`'\n  sources:\n  - openapi/chrome-river-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chrome-river/refs/heads/main/authentication/chrome-river-authentication.yml
summary_line: http · 1 scheme
tags:
- Finance
- Expense Management
- SaaS
- Enterprise
- Travel
---
