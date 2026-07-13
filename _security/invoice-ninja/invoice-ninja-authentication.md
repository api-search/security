---
api_key_in:
- header
api_specs:
- filename: invoiceninja
  format: yaml
  label: Invoice Ninja v5 API
  slug: v5-api
  spec_type: OpenAPI
  url: https://app.swaggerhub.com/apis/invoiceninja/invoiceninja
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
- Open Source
- Freelancers
- SMB
---
