---
api_key_in: []
api_specs:
- filename: amex-gbt-user-sync-api-openapi.json
  format: json
  label: Egencia User Sync API
  slug: egencia-user-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-user-sync-api-openapi.json
- filename: amex-gbt-sso-context-api-openapi.json
  format: json
  label: Egencia Context SSO API
  slug: egencia-context-sso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-sso-context-api-openapi.json
- filename: amex-gbt-company-info-api-openapi.json
  format: json
  label: Egencia Company Details API
  slug: egencia-company-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-company-info-api-openapi.json
- filename: amex-gbt-company-cdf-api-openapi.json
  format: json
  label: Egencia Company CDF API
  slug: egencia-company-cdf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-company-cdf-api-openapi.json
- filename: amex-gbt-validation-spi-openapi.json
  format: json
  label: Egencia Validation SPI
  slug: egencia-validation-spi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-validation-spi-openapi.json
- filename: amex-gbt-expense-spi-openapi.json
  format: json
  label: Egencia Expense SPI
  slug: egencia-expense-spi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-expense-spi-openapi.json
- filename: amex-gbt-booking-api-openapi.json
  format: json
  label: Egencia Get Booking API
  slug: egencia-get-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-booking-api-openapi.json
- filename: amex-gbt-cancellation-deletion-api-openapi.json
  format: json
  label: Egencia Expense Cancellation and Deletion API
  slug: egencia-cancellation-deletion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-cancellation-deletion-api-openapi.json
- filename: amex-gbt-approval-workflow-api-openapi.json
  format: json
  label: Egencia Approval Workflow API
  slug: egencia-approval-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-approval-workflow-api-openapi.json
- filename: amex-gbt-approval-customisation-spi-openapi.json
  format: json
  label: Egencia Approval Customisation SPI
  slug: egencia-approval-customisation-spi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-approval-customisation-spi-openapi.json
- filename: amex-gbt-receipt-api-openapi.json
  format: json
  label: Egencia Receipt API
  slug: egencia-receipt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-receipt-api-openapi.json
- filename: amex-gbt-duty-of-care-api-openapi.json
  format: json
  label: Egencia Duty of Care API
  slug: egencia-duty-of-care-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-duty-of-care-api-openapi.json
- filename: amex-gbt-reporting-api-openapi.json
  format: json
  label: Egencia Reporting API (BI Transactions)
  slug: egencia-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-reporting-api-openapi.json
- filename: amex-gbt-service-bi-openapi.json
  format: json
  label: American Express Global Business Travel BI API
  slug: amex-gbt-service-bi-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-service-bi-openapi.json
- filename: amex-gbt-service-company-openapi.json
  format: json
  label: American Express Global Business Travel OpenAPI definition (Amex Gbt Service Company)
  slug: amex-gbt-service-company-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-service-company-openapi.json
- filename: amex-gbt-service-dutyofcare-openapi.json
  format: json
  label: American Express Global Business Travel Duty Of Care API
  slug: amex-gbt-service-dutyofcare-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-service-dutyofcare-openapi.json
- filename: amex-gbt-service-openconnect-openapi.json
  format: json
  label: American Express Global Business Travel OpenAPI definition (Amex Gbt Service Openconnect)
  slug: amex-gbt-service-openconnect-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-service-openconnect-openapi.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Amex Gbt Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: American Express Global Business Travel secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: American Express Global Business Travel
provider_slug: amex-gbt
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://apis.egencia.com/auth/v1/token
  name: OAuth2
  sources:
  - openapi/amex-gbt-approval-workflow-api-openapi.json
  - openapi/amex-gbt-booking-api-openapi.json
  - openapi/amex-gbt-cancellation-deletion-api-openapi.json
  - openapi/amex-gbt-company-cdf-api-openapi.json
  - openapi/amex-gbt-company-info-api-openapi.json
  - openapi/amex-gbt-duty-of-care-api-openapi.json
  - openapi/amex-gbt-receipt-api-openapi.json
  - openapi/amex-gbt-reporting-api-openapi.json
  - openapi/amex-gbt-service-bi-openapi.json
  - openapi/amex-gbt-service-company-openapi.json
  - openapi/amex-gbt-service-dutyofcare-openapi.json
  - openapi/amex-gbt-service-openconnect-openapi.json
  - openapi/amex-gbt-user-sync-api-openapi.json
  type: oauth2
slug: amex-gbt-authentication
source_filename: amex-gbt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: derived\nsource: openapi/amex-gbt-approval-workflow-api-openapi.json, openapi/amex-gbt-booking-api-openapi.json,\n  openapi/amex-gbt-cancellation-deletion-api-openapi.json, openapi/amex-gbt-company-cdf-api-openapi.json,\n  openapi/amex-gbt-company-info-api-openapi.json, openapi/amex-gbt-duty-of-care-api-openapi.json,\n  openapi/amex-gbt-receipt-api-openapi.json, openapi/amex-gbt-reporting-api-openapi.json, openapi/amex-gbt-service-bi-openapi.json,\n  openapi/amex-gbt-service-company-openapi.json, openapi/amex-gbt-service-dutyofcare-openapi.json,\n  openapi/amex-gbt-service-openconnect-openapi.json ...\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.egencia.com/auth/v1/token\n    scopes: 0\n  sources:\n  - openapi/amex-gbt-approval-workflow-api-openapi.json\n  - openapi/amex-gbt-booking-api-openapi.json\n  - openapi/amex-gbt-cancellation-deletion-api-openapi.json\n\
  \  - openapi/amex-gbt-company-cdf-api-openapi.json\n  - openapi/amex-gbt-company-info-api-openapi.json\n  - openapi/amex-gbt-duty-of-care-api-openapi.json\n  - openapi/amex-gbt-receipt-api-openapi.json\n  - openapi/amex-gbt-reporting-api-openapi.json\n  - openapi/amex-gbt-service-bi-openapi.json\n  - openapi/amex-gbt-service-company-openapi.json\n  - openapi/amex-gbt-service-dutyofcare-openapi.json\n  - openapi/amex-gbt-service-openconnect-openapi.json\n  - openapi/amex-gbt-user-sync-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/authentication/amex-gbt-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Travel
- United States
- Corporate Travel
- Travel Management
- Business Travel
- Distribution
- Booking
- Aviation
- Hotels
- Rail
- Car Rental
- Expense
- Duty of Care
- Reporting
---
