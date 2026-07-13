---
api_key_in: []
api_specs:
- filename: tabs-platform-openapi.yml
  format: yaml
  label: Tabs Contracts API
  slug: tabs-platform-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabs-platform/refs/heads/main/openapi/tabs-platform-openapi.yml
- filename: tabs-platform-openapi.yml
  format: yaml
  label: Tabs Invoices API
  slug: tabs-platform-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabs-platform/refs/heads/main/openapi/tabs-platform-openapi.yml
- filename: tabs-platform-openapi.yml
  format: yaml
  label: Tabs Revenue Recognition API
  slug: tabs-platform-revenue-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabs-platform/refs/heads/main/openapi/tabs-platform-openapi.yml
- filename: tabs-platform-openapi.yml
  format: yaml
  label: Tabs Payments API
  slug: tabs-platform-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabs-platform/refs/heads/main/openapi/tabs-platform-openapi.yml
- filename: tabs-platform-openapi.yml
  format: yaml
  label: Tabs Customers API
  slug: tabs-platform-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabs-platform/refs/heads/main/openapi/tabs-platform-openapi.yml
- filename: tabs-platform-openapi.yml
  format: yaml
  label: Tabs Usage Events API
  slug: tabs-platform-usage-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabs-platform/refs/heads/main/openapi/tabs-platform-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: sourced
name: Tabs Platform Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tabs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tabs
provider_slug: tabs-platform
scheme_count: 1
schemes:
- description: 'API key passed directly in the Authorization header (`Authorization: YOUR_API_KEY`, no Bearer prefix). Keys are created in the Developers section of the Tabs app and require administrator privileges; non-admins must contact their Tabs administrator. Keys should be treated as confidential; self-service key rotation is noted as a planned capability.'
  in: header
  name: apiKeyAuth
  scheme: none
  sources:
  - https://docs.tabsplatform.com/docs/authentication
  type: apiKey
slug: tabs-platform-authentication
source_filename: tabs-platform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: sourced\nsource: https://docs.tabsplatform.com/docs/authentication\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  scheme: none\n  description: >-\n    API key passed directly in the Authorization header\n    (`Authorization: YOUR_API_KEY`, no Bearer prefix). Keys are created in the\n    Developers section of the Tabs app and require administrator privileges;\n    non-admins must contact their Tabs administrator. Keys should be treated as\n    confidential; self-service key rotation is noted as a planned capability.\n  sources:\n  - https://docs.tabsplatform.com/docs/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tabs-platform/refs/heads/main/authentication/tabs-platform-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Revenue Recognition
- ASC 606
- Billing
- B2B Payments
- Accounts Receivable
- Invoicing
- Collections
- Usage-Based Billing
- Subscriptions
- Contracts
- Finance
- Revenue Automation
---
