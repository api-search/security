---
api_key_in: []
api_specs:
- filename: ppro-authorization-endpoints-api-openapi.yml
  format: yaml
  label: PPRO Authorization Endpoints API
  slug: ppro-authorization-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-authorization-endpoints-api-openapi.yml
- filename: ppro-capture-endpoints-api-openapi.yml
  format: yaml
  label: PPRO Capture Endpoints API
  slug: ppro-capture-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-capture-endpoints-api-openapi.yml
- filename: ppro-dispute-reports-api-openapi.yml
  format: yaml
  label: PPRO Dispute Reports API
  slug: ppro-dispute-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-dispute-reports-api-openapi.yml
- filename: ppro-disputes-api-openapi.yml
  format: yaml
  label: PPRO Disputes API
  slug: ppro-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-disputes-api-openapi.yml
- filename: ppro-enrollment-endpoints-api-openapi.yml
  format: yaml
  label: PPRO Enrollment Endpoints API
  slug: ppro-enrollment-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-enrollment-endpoints-api-openapi.yml
- filename: ppro-internal-api-openapi.yml
  format: yaml
  label: PPRO Internal API
  slug: ppro-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-internal-api-openapi.yml
- filename: ppro-merchants-api-openapi.yml
  format: yaml
  label: PPRO Merchants API
  slug: ppro-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-merchants-api-openapi.yml
- filename: ppro-payment-agreement-revocations-api-openapi.yml
  format: yaml
  label: PPRO Payment Agreement Revocations API
  slug: ppro-payment-agreement-revocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-payment-agreement-revocations-api-openapi.yml
- filename: ppro-payment-agreements-api-openapi.yml
  format: yaml
  label: PPRO Payment Agreements API
  slug: ppro-payment-agreements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-payment-agreements-api-openapi.yml
- filename: ppro-payment-charge-controller-api-openapi.yml
  format: yaml
  label: PPRO Payment Charge Controller API
  slug: ppro-payment-charge-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-payment-charge-controller-api-openapi.yml
- filename: ppro-payment-charges-api-openapi.yml
  format: yaml
  label: PPRO Payment Charges API
  slug: ppro-payment-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-payment-charges-api-openapi.yml
- filename: ppro-payment-instruments-api-openapi.yml
  format: yaml
  label: PPRO Payment Instruments API
  slug: ppro-payment-instruments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-payment-instruments-api-openapi.yml
- filename: ppro-payment-sessions-api-openapi.yml
  format: yaml
  label: PPRO Payment Sessions API
  slug: ppro-payment-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-payment-sessions-api-openapi.yml
- filename: ppro-people-api-openapi.yml
  format: yaml
  label: PPRO People API
  slug: ppro-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-people-api-openapi.yml
- filename: ppro-platforms-api-openapi.yml
  format: yaml
  label: PPRO Platforms API
  slug: ppro-platforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-platforms-api-openapi.yml
- filename: ppro-psps-api-openapi.yml
  format: yaml
  label: PPRO PS Ps API
  slug: ppro-psps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-psps-api-openapi.yml
- filename: ppro-refund-endpoints-api-openapi.yml
  format: yaml
  label: PPRO Refund Endpoints API
  slug: ppro-refund-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-refund-endpoints-api-openapi.yml
- filename: ppro-void-endpoints-api-openapi.yml
  format: yaml
  label: PPRO Void Endpoints API
  slug: ppro-void-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-void-endpoints-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ppro Authentication
name_suffix: Authentication
oauth_flows: []
overview: PPRO secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PPRO
provider_slug: ppro
scheme_count: 1
schemes:
- name: bearer_token
  scheme: bearer
  sources:
  - openapi/ppro-payment-agreements-openapi.yml
  - openapi/ppro-payment-charges-openapi.yml
  - openapi/ppro-payment-instruments-openapi.yml
  - openapi/ppro-payment-sessions-openapi.yml
  type: http
slug: ppro-authentication
source_filename: ppro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: derived\nsource: openapi/ppro-payment-agreements-openapi.yml, openapi/ppro-payment-charges-openapi.yml,\n  openapi/ppro-payment-instruments-openapi.yml, openapi/ppro-payment-sessions-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer_token\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/ppro-payment-agreements-openapi.yml\n  - openapi/ppro-payment-charges-openapi.yml\n  - openapi/ppro-payment-instruments-openapi.yml\n  - openapi/ppro-payment-sessions-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/authentication/ppro-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Local Payment Methods
- Financial Services
- Fintech
- Acquiring
- Checkout
- E-commerce
- Digital Wallets
- Recurring Payments
- Disputes
- Chargebacks
- Company
---
