---
api_key_in:
- header
api_specs:
- filename: invoice-ninja-activities-api-openapi.yml
  format: yaml
  label: Invoice Ninja Activities API
  slug: invoice-ninja-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invoice-ninja/refs/heads/main/openapi/invoice-ninja-activities-api-openapi.yml
- filename: invoice-ninja-authentication-api-openapi.yml
  format: yaml
  label: Invoice Ninja Authentication API
  slug: invoice-ninja-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invoice-ninja/refs/heads/main/openapi/invoice-ninja-authentication-api-openapi.yml
- filename: invoice-ninja-bank-integrations-api-openapi.yml
  format: yaml
  label: Invoice Ninja Bank Integrations API
  slug: invoice-ninja-bank-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invoice-ninja/refs/heads/main/openapi/invoice-ninja-bank-integrations-api-openapi.yml
- filename: invoice-ninja-bank-transaction-rules-api-openapi.yml
  format: yaml
  label: Invoice Ninja Bank Transaction Rules API
  slug: invoice-ninja-bank-transaction-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invoice-ninja/refs/heads/main/openapi/invoice-ninja-bank-transaction-rules-api-openapi.yml
- filename: invoice-ninja-bank-transactions-api-openapi.yml
  format: yaml
  label: Invoice Ninja Bank Transactions API
  slug: invoice-ninja-bank-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invoice-ninja/refs/heads/main/openapi/invoice-ninja-bank-transactions-api-openapi.yml
- filename: invoice-ninja-charts-api-openapi.yml
  format: yaml
  label: Invoice Ninja Charts API
  slug: invoice-ninja-charts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invoice-ninja/refs/heads/main/openapi/invoice-ninja-charts-api-openapi.yml
- filename: invoice-ninja-client-gateway-tokens-api-openapi.yml
  format: yaml
  label: Invoice Ninja Client Gateway Tokens API
  slug: invoice-ninja-client-gateway-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invoice-ninja/refs/heads/main/openapi/invoice-ninja-client-gateway-tokens-api-openapi.yml
- filename: invoice-ninja-companies-api-openapi.yml
  format: yaml
  label: Invoice Ninja Companies API
  slug: invoice-ninja-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invoice-ninja/refs/heads/main/openapi/invoice-ninja-companies-api-openapi.yml
- filename: invoice-ninja-company-gateways-api-openapi.yml
  format: yaml
  label: Invoice Ninja Company Gateways API
  slug: invoice-ninja-company-gateways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invoice-ninja/refs/heads/main/openapi/invoice-ninja-company-gateways-api-openapi.yml
- filename: invoice-ninja-settings-api-openapi.yml
  format: yaml
  label: Invoice Ninja Settings API
  slug: invoice-ninja-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invoice-ninja/refs/heads/main/openapi/invoice-ninja-settings-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Invoice Ninja Authentication
name_suffix: Authentication
oauth_flows: []
overview: Invoice Ninja secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Invoice Ninja
provider_slug: invoice-ninja
scheme_count: 1
schemes:
- description: 'API token created in the Invoice Ninja settings. Self-hosted installs

    may additionally require an `X-Api-Secret` header.'
  in: header
  name: apiToken
  parameter: X-Api-Token
  sources:
  - openapi/invoice-ninja-openapi.yml
  type: apiKey
slug: invoice-ninja-authentication
source_filename: invoice-ninja-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/invoice-ninja-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiToken\n  type: apiKey\n  in: header\n  parameter: X-Api-Token\n  description: |-\n    API token created in the Invoice Ninja settings. Self-hosted installs\n    may additionally require an `X-Api-Secret` header.\n  sources:\n  - openapi/invoice-ninja-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/invoice-ninja/refs/heads/main/authentication/invoice-ninja-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Invoicing
- Billing
- Payments
- Accounting
- Open-Source
- Freelancers
- SMB
---
