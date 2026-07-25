---
api_key_in: []
api_specs:
- filename: lexoffice-contacts-api-openapi.yml
  format: yaml
  label: lexoffice Contacts API
  slug: lexoffice-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-contacts-api-openapi.yml
- filename: lexoffice-credit-notes-api-openapi.yml
  format: yaml
  label: lexoffice Credit Notes API
  slug: lexoffice-credit-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-credit-notes-api-openapi.yml
- filename: lexoffice-delivery-notes-api-openapi.yml
  format: yaml
  label: lexoffice Delivery Notes API
  slug: lexoffice-delivery-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-delivery-notes-api-openapi.yml
- filename: lexoffice-down-payment-invoices-api-openapi.yml
  format: yaml
  label: lexoffice Down Payment Invoices API
  slug: lexoffice-down-payment-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-down-payment-invoices-api-openapi.yml
- filename: lexoffice-dunnings-api-openapi.yml
  format: yaml
  label: lexoffice Dunnings API
  slug: lexoffice-dunnings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-dunnings-api-openapi.yml
- filename: lexoffice-event-subscriptions-api-openapi.yml
  format: yaml
  label: lexoffice Event Subscriptions API
  slug: lexoffice-event-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-event-subscriptions-api-openapi.yml
- filename: lexoffice-files-api-openapi.yml
  format: yaml
  label: lexoffice Files API
  slug: lexoffice-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-files-api-openapi.yml
- filename: lexoffice-invoices-api-openapi.yml
  format: yaml
  label: lexoffice Invoices API
  slug: lexoffice-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-invoices-api-openapi.yml
- filename: lexoffice-order-confirmations-api-openapi.yml
  format: yaml
  label: lexoffice Order Confirmations API
  slug: lexoffice-order-confirmations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-order-confirmations-api-openapi.yml
- filename: lexoffice-payments-api-openapi.yml
  format: yaml
  label: lexoffice Payments API
  slug: lexoffice-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-payments-api-openapi.yml
- filename: lexoffice-profile-api-openapi.yml
  format: yaml
  label: lexoffice Profile API
  slug: lexoffice-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-profile-api-openapi.yml
- filename: lexoffice-quotations-api-openapi.yml
  format: yaml
  label: lexoffice Quotations API
  slug: lexoffice-quotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-quotations-api-openapi.yml
- filename: lexoffice-recurring-templates-api-openapi.yml
  format: yaml
  label: lexoffice Recurring Templates API
  slug: lexoffice-recurring-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-recurring-templates-api-openapi.yml
- filename: lexoffice-vouchers-api-openapi.yml
  format: yaml
  label: lexoffice Vouchers API
  slug: lexoffice-vouchers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-vouchers-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lexoffice Authentication
name_suffix: Authentication
oauth_flows: []
overview: lexoffice secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: lexoffice
provider_slug: lexoffice
scheme_count: 1
schemes:
- description: 'Bearer API key. The account owner generates a private API key from the Public API add-on at https://app.lexware.de/addons/public-api (self-serve; requires a paid lexoffice / lexware Office plan) and passes it as `Authorization: Bearer YOUR_API_KEY` on every request. The key is a long-lived token scoped to the connected organization. There is no OAuth client registration or partner application for the standard REST API.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/lexoffice-openapi.yml
  - https://developers.lexware.io/docs/
  - https://app.lexware.de/addons/public-api
  type: http
slug: lexoffice-authentication
source_filename: lexoffice-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/lexoffice-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer API key. The account owner generates a private API key from the Public\n    API add-on at https://app.lexware.de/addons/public-api (self-serve; requires a\n    paid lexoffice / lexware Office plan) and passes it as `Authorization: Bearer\n    YOUR_API_KEY` on every request. The key is a long-lived token scoped to the\n    connected organization. There is no OAuth client registration or partner\n    application for the standard REST API.\n  sources:\n  - openapi/lexoffice-openapi.yml\n  - https://developers.lexware.io/docs/\n  - https://app.lexware.de/addons/public-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/authentication/lexoffice-authentication.yml
summary_line: http · 1 scheme
tags:
- Accounting
- Invoicing
- Bookkeeping
- Finance
- Germany
- Vouchers
- Contacts
- SaaS
- Financial Software
---
