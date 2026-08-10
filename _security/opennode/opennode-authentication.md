---
api_key_in:
- header
api_specs:
- filename: opennode-charges-api-openapi.yml
  format: yaml
  label: OpenNode Charges API
  slug: opennode-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opennode/refs/heads/main/openapi/opennode-charges-api-openapi.yml
- filename: opennode-withdrawals-api-openapi.yml
  format: yaml
  label: OpenNode Withdrawals API
  slug: opennode-withdrawals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opennode/refs/heads/main/openapi/opennode-withdrawals-api-openapi.yml
- filename: opennode-refunds-api-openapi.yml
  format: yaml
  label: OpenNode Refunds API
  slug: opennode-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opennode/refs/heads/main/openapi/opennode-refunds-api-openapi.yml
- filename: opennode-account-api-openapi.yml
  format: yaml
  label: OpenNode Account API
  slug: opennode-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opennode/refs/heads/main/openapi/opennode-account-api-openapi.yml
- filename: opennode-static-addresses-api-openapi.yml
  format: yaml
  label: OpenNode Static Addresses API
  slug: opennode-static-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opennode/refs/heads/main/openapi/opennode-static-addresses-api-openapi.yml
- filename: opennode-account-api-openapi.yml
  format: yaml
  label: OpenNode Account API
  slug: opennode-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opennode/refs/heads/main/openapi/opennode-account-api-openapi.yml
- filename: opennode-charges-api-openapi.yml
  format: yaml
  label: OpenNode Charges API
  slug: opennode-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opennode/refs/heads/main/openapi/opennode-charges-api-openapi.yml
- filename: opennode-rates-api-openapi.yml
  format: yaml
  label: OpenNode Rates API
  slug: opennode-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opennode/refs/heads/main/openapi/opennode-rates-api-openapi.yml
- filename: opennode-refunds-api-openapi.yml
  format: yaml
  label: OpenNode Refunds API
  slug: opennode-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opennode/refs/heads/main/openapi/opennode-refunds-api-openapi.yml
- filename: opennode-static-addresses-api-openapi.yml
  format: yaml
  label: OpenNode Static Addresses API
  slug: opennode-static-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opennode/refs/heads/main/openapi/opennode-static-addresses-api-openapi.yml
- filename: opennode-withdrawals-api-openapi.yml
  format: yaml
  label: OpenNode Withdrawals API
  slug: opennode-withdrawals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opennode/refs/heads/main/openapi/opennode-withdrawals-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Opennode Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenNode secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenNode
provider_slug: opennode
scheme_count: 1
schemes:
- description: API key obtained from the OpenNode dashboard. Pass the key directly in the Authorization header (no "Bearer" prefix required).
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/opennode-openapi.yml
  type: apiKey
slug: opennode-authentication
source_filename: opennode-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/opennode-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key obtained from the OpenNode dashboard. Pass the key directly in the Authorization\n    header (no \"Bearer\" prefix required).\n  sources:\n  - openapi/opennode-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opennode/refs/heads/main/authentication/opennode-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Bitcoin
- Lightning Network
- Payments
- Payment Processing
- Cryptocurrency
- Fintech
- Webhooks
- Invoicing
- Payouts
- LNURL
---
