---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lynx-investments-api-openapi.yml
  format: yaml
  label: Lynx Investments API
  slug: lynx-investments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lynx/refs/heads/main/openapi/lynx-investments-api-openapi.yml
- filename: lynx-tags-api-openapi.yml
  format: yaml
  label: Lynx Tags API
  slug: lynx-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lynx/refs/heads/main/openapi/lynx-tags-api-openapi.yml
- filename: lynx-accounts-api-openapi.yml
  format: yaml
  label: Lynx Accounts API
  slug: lynx-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lynx/refs/heads/main/openapi/lynx-accounts-api-openapi.yml
- filename: lynx-cards-api-openapi.yml
  format: yaml
  label: Lynx Cards API
  slug: lynx-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lynx/refs/heads/main/openapi/lynx-cards-api-openapi.yml
- filename: lynx-claims-api-openapi.yml
  format: yaml
  label: Lynx Claims API
  slug: lynx-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lynx/refs/heads/main/openapi/lynx-claims-api-openapi.yml
- filename: lynx-client-org-application-token-controller-api-openapi.yml
  format: yaml
  label: Lynx Client Org Application Token Controller API
  slug: lynx-client-org-application-token-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lynx/refs/heads/main/openapi/lynx-client-org-application-token-controller-api-openapi.yml
- filename: lynx-clients-api-openapi.yml
  format: yaml
  label: Lynx Clients API
  slug: lynx-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lynx/refs/heads/main/openapi/lynx-clients-api-openapi.yml
- filename: lynx-commerce-api-openapi.yml
  format: yaml
  label: Lynx Commerce API
  slug: lynx-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lynx/refs/heads/main/openapi/lynx-commerce-api-openapi.yml
- filename: lynx-copay-api-openapi.yml
  format: yaml
  label: Lynx Copay API
  slug: lynx-copay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lynx/refs/heads/main/openapi/lynx-copay-api-openapi.yml
- filename: lynx-enrollments-api-openapi.yml
  format: yaml
  label: Lynx Enrollments API
  slug: lynx-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lynx/refs/heads/main/openapi/lynx-enrollments-api-openapi.yml
- filename: lynx-expense-api-openapi.yml
  format: yaml
  label: Lynx Expense API
  slug: lynx-expense-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lynx/refs/heads/main/openapi/lynx-expense-api-openapi.yml
- filename: lynx-externalaccounts-api-openapi.yml
  format: yaml
  label: Lynx Externalaccounts API
  slug: lynx-externalaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lynx/refs/heads/main/openapi/lynx-externalaccounts-api-openapi.yml
- filename: lynx-externalnotifications-api-openapi.yml
  format: yaml
  label: Lynx Externalnotifications API
  slug: lynx-externalnotifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lynx/refs/heads/main/openapi/lynx-externalnotifications-api-openapi.yml
- filename: lynx-member-expense-controller-api-openapi.yml
  format: yaml
  label: Lynx Member Expense Controller API
  slug: lynx-member-expense-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lynx/refs/heads/main/openapi/lynx-member-expense-controller-api-openapi.yml
- filename: lynx-members-api-openapi.yml
  format: yaml
  label: Lynx Members API
  slug: lynx-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lynx/refs/heads/main/openapi/lynx-members-api-openapi.yml
- filename: lynx-payments-api-openapi.yml
  format: yaml
  label: Lynx Payments API
  slug: lynx-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lynx/refs/heads/main/openapi/lynx-payments-api-openapi.yml
- filename: lynx-relatedpersons-api-openapi.yml
  format: yaml
  label: Lynx Relatedpersons API
  slug: lynx-relatedpersons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lynx/refs/heads/main/openapi/lynx-relatedpersons-api-openapi.yml
- filename: lynx-substantiation-api-openapi.yml
  format: yaml
  label: Lynx Substantiation API
  slug: lynx-substantiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lynx/refs/heads/main/openapi/lynx-substantiation-api-openapi.yml
- filename: lynx-transactions-api-openapi.yml
  format: yaml
  label: Lynx Transactions API
  slug: lynx-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lynx/refs/heads/main/openapi/lynx-transactions-api-openapi.yml
- filename: lynx-uploads-api-openapi.yml
  format: yaml
  label: Lynx Uploads API
  slug: lynx-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lynx/refs/heads/main/openapi/lynx-uploads-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Lynx Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lynx secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lynx
provider_slug: lynx
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/lynx-account-api-openapi.yml
  - openapi/lynx-card-management-api-openapi.yml
  - openapi/lynx-claims-service-api-openapi.yml
  - openapi/lynx-client-org-management-api-openapi.yml
  - openapi/lynx-commerce-order-api-openapi.yml
  - openapi/lynx-commodity-api-openapi.yml
  - openapi/lynx-copay-management-service-api-openapi.yml
  - openapi/lynx-enrollment-api-openapi.yml
  - openapi/lynx-external-account-api-openapi.yml
  - openapi/lynx-external-notification-api-openapi.yml
  - openapi/lynx-investments-api-openapi.yml
  - openapi/lynx-member-management-api-openapi.yml
  - openapi/lynx-payment-api-openapi.yml
  - openapi/lynx-related-person-api-openapi.yml
  - openapi/lynx-substantiation-service-api-openapi.yml
  - openapi/lynx-tags-api-openapi.yml
  - openapi/lynx-transaction-api-openapi.yml
  - openapi/lynx-upload-api-openapi.yml
  type: http
slug: lynx-authentication
source_filename: lynx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: derived\nsource: openapi/lynx-account-api-openapi.yml, openapi/lynx-card-management-api-openapi.yml,\n  openapi/lynx-claims-service-api-openapi.yml, openapi/lynx-client-org-management-api-openapi.yml,\n  openapi/lynx-commerce-order-api-openapi.yml, openapi/lynx-commodity-api-openapi.yml, openapi/lynx-copay-management-service-api-openapi.yml,\n  openapi/lynx-enrollment-api-openapi.yml, openapi/lynx-external-account-api-openapi.yml, openapi/lynx-external-notification-api-openapi.yml,\n  openapi/lynx-investments-api-openapi.yml, openapi/lynx-member-management-api-openapi.yml ...\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/lynx-account-api-openapi.yml\n  - openapi/lynx-card-management-api-openapi.yml\n  - openapi/lynx-claims-service-api-openapi.yml\n  - openapi/lynx-client-org-management-api-openapi.yml\n  - openapi/lynx-commerce-order-api-openapi.yml\n\
  \  - openapi/lynx-commodity-api-openapi.yml\n  - openapi/lynx-copay-management-service-api-openapi.yml\n  - openapi/lynx-enrollment-api-openapi.yml\n  - openapi/lynx-external-account-api-openapi.yml\n  - openapi/lynx-external-notification-api-openapi.yml\n  - openapi/lynx-investments-api-openapi.yml\n  - openapi/lynx-member-management-api-openapi.yml\n  - openapi/lynx-payment-api-openapi.yml\n  - openapi/lynx-related-person-api-openapi.yml\n  - openapi/lynx-substantiation-service-api-openapi.yml\n  - openapi/lynx-tags-api-openapi.yml\n  - openapi/lynx-transaction-api-openapi.yml\n  - openapi/lynx-upload-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lynx/refs/heads/main/authentication/lynx-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Healthcare
- Fintech
- Payments
- Benefits
- Health Savings Accounts
- Embedded Finance
- Card Issuing
- Insurance
---
