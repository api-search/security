---
api_key_in: []
api_specs:
- filename: sap-sd-sales-order-openapi.yml
  format: yaml
  label: Sales Order API
  slug: sales-order
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-sales-order-openapi.yml
- filename: sap-sd-customer-master-data-openapi.yml
  format: yaml
  label: Customer Master Data API
  slug: customer-master-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-customer-master-data-openapi.yml
- filename: sap-sd-outbound-delivery-openapi.yml
  format: yaml
  label: Outbound Delivery API
  slug: outbound-delivery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-outbound-delivery-openapi.yml
- filename: sap-sd-billing-document-openapi.yml
  format: yaml
  label: Billing Document API
  slug: billing-document
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-billing-document-openapi.yml
- filename: sap-sd-pricing-openapi.yml
  format: yaml
  label: Pricing API
  slug: pricing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-pricing-openapi.yml
- filename: sap-sd-sales-quotation-openapi.yml
  format: yaml
  label: Sales Quotation API
  slug: sales-quotation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-sales-quotation-openapi.yml
- filename: sap-sd-credit-management-openapi.yml
  format: yaml
  label: Credit Management API
  slug: credit-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-credit-management-openapi.yml
- filename: sap-sd-material-master-openapi.yml
  format: yaml
  label: Material Master API
  slug: material-master
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-material-master-openapi.yml
- filename: sap-sd-credit-memo-request-openapi.yml
  format: yaml
  label: Credit Memo Request API
  slug: credit-memo-request
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-credit-memo-request-openapi.yml
- filename: sap-sd-debit-memo-request-openapi.yml
  format: yaml
  label: Debit Memo Request API
  slug: debit-memo-request
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-debit-memo-request-openapi.yml
- filename: sap-sd-sales-contract-openapi.yml
  format: yaml
  label: Sales Contract API
  slug: sales-contract
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-sales-contract-openapi.yml
- filename: sap-sd-sales-inquiry-openapi.yml
  format: yaml
  label: Sales Inquiry API
  slug: sales-inquiry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-sales-inquiry-openapi.yml
- filename: sap-sd-sales-scheduling-agreement-openapi.yml
  format: yaml
  label: Sales Scheduling Agreement API
  slug: sales-scheduling-agreement
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-sales-scheduling-agreement-openapi.yml
- filename: sap-sd-customer-return-openapi.yml
  format: yaml
  label: Customer Return API
  slug: customer-return
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-customer-return-openapi.yml
- filename: sap-sd-customer-returns-delivery-openapi.yml
  format: yaml
  label: Customer Returns Delivery API
  slug: customer-returns-delivery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-customer-returns-delivery-openapi.yml
- filename: sap-sd-customer-material-openapi.yml
  format: yaml
  label: Customer Material API
  slug: customer-material
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-customer-material-openapi.yml
- filename: sap-sd-inbound-delivery-openapi.yml
  format: yaml
  label: Inbound Delivery API
  slug: inbound-delivery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-inbound-delivery-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Sap Sales And Distribution Sd Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: SAP Sales and Distribution (SD) secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: SAP Sales and Distribution (SD)
provider_slug: sap-sales-and-distribution-sd
scheme_count: 2
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/sap-sd-billing-document-openapi.yml
  - openapi/sap-sd-credit-management-openapi.yml
  - openapi/sap-sd-credit-memo-request-openapi.yml
  - openapi/sap-sd-customer-master-data-openapi.yml
  - openapi/sap-sd-customer-material-openapi.yml
  - openapi/sap-sd-customer-return-openapi.yml
  - openapi/sap-sd-customer-returns-delivery-openapi.yml
  - openapi/sap-sd-debit-memo-request-openapi.yml
  - openapi/sap-sd-inbound-delivery-openapi.yml
  - openapi/sap-sd-material-master-openapi.yml
  - openapi/sap-sd-outbound-delivery-openapi.yml
  - openapi/sap-sd-pricing-openapi.yml
  - openapi/sap-sd-sales-contract-openapi.yml
  - openapi/sap-sd-sales-inquiry-openapi.yml
  - openapi/sap-sd-sales-order-openapi.yml
  - openapi/sap-sd-sales-quotation-openapi.yml
  - openapi/sap-sd-sales-scheduling-agreement-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token
  name: oauth2
  sources:
  - openapi/sap-sd-billing-document-openapi.yml
  - openapi/sap-sd-credit-management-openapi.yml
  - openapi/sap-sd-credit-memo-request-openapi.yml
  - openapi/sap-sd-customer-master-data-openapi.yml
  - openapi/sap-sd-customer-material-openapi.yml
  - openapi/sap-sd-customer-return-openapi.yml
  - openapi/sap-sd-customer-returns-delivery-openapi.yml
  - openapi/sap-sd-debit-memo-request-openapi.yml
  - openapi/sap-sd-inbound-delivery-openapi.yml
  - openapi/sap-sd-material-master-openapi.yml
  - openapi/sap-sd-outbound-delivery-openapi.yml
  - openapi/sap-sd-pricing-openapi.yml
  - openapi/sap-sd-sales-contract-openapi.yml
  - openapi/sap-sd-sales-inquiry-openapi.yml
  - openapi/sap-sd-sales-order-openapi.yml
  - openapi/sap-sd-sales-quotation-openapi.yml
  - openapi/sap-sd-sales-scheduling-agreement-openapi.yml
  type: oauth2
slug: sap-sales-and-distribution-sd-authentication
source_filename: sap-sales-and-distribution-sd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sap-sd-billing-document-openapi.yml, openapi/sap-sd-credit-management-openapi.yml,\n  openapi/sap-sd-credit-memo-request-openapi.yml, openapi/sap-sd-customer-master-data-openapi.yml,\n  openapi/sap-sd-customer-material-openapi.yml, openapi/sap-sd-customer-return-openapi.yml,\n  openapi/sap-sd-customer-returns-delivery-openapi.yml, openapi/sap-sd-debit-memo-request-openapi.yml,\n  openapi/sap-sd-inbound-delivery-openapi.yml, openapi/sap-sd-material-master-openapi.yml, openapi/sap-sd-outbound-delivery-openapi.yml,\n  openapi/sap-sd-pricing-openapi.yml ...\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/sap-sd-billing-document-openapi.yml\n  - openapi/sap-sd-credit-management-openapi.yml\n  - openapi/sap-sd-credit-memo-request-openapi.yml\n  - openapi/sap-sd-customer-master-data-openapi.yml\n  - openapi/sap-sd-customer-material-openapi.yml\n\
  \  - openapi/sap-sd-customer-return-openapi.yml\n  - openapi/sap-sd-customer-returns-delivery-openapi.yml\n  - openapi/sap-sd-debit-memo-request-openapi.yml\n  - openapi/sap-sd-inbound-delivery-openapi.yml\n  - openapi/sap-sd-material-master-openapi.yml\n  - openapi/sap-sd-outbound-delivery-openapi.yml\n  - openapi/sap-sd-pricing-openapi.yml\n  - openapi/sap-sd-sales-contract-openapi.yml\n  - openapi/sap-sd-sales-inquiry-openapi.yml\n  - openapi/sap-sd-sales-order-openapi.yml\n  - openapi/sap-sd-sales-quotation-openapi.yml\n  - openapi/sap-sd-sales-scheduling-agreement-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token\n    scopes: 1\n  sources:\n  - openapi/sap-sd-billing-document-openapi.yml\n  - openapi/sap-sd-credit-management-openapi.yml\n  - openapi/sap-sd-credit-memo-request-openapi.yml\n  - openapi/sap-sd-customer-master-data-openapi.yml\n  - openapi/sap-sd-customer-material-openapi.yml\n\
  \  - openapi/sap-sd-customer-return-openapi.yml\n  - openapi/sap-sd-customer-returns-delivery-openapi.yml\n  - openapi/sap-sd-debit-memo-request-openapi.yml\n  - openapi/sap-sd-inbound-delivery-openapi.yml\n  - openapi/sap-sd-material-master-openapi.yml\n  - openapi/sap-sd-outbound-delivery-openapi.yml\n  - openapi/sap-sd-pricing-openapi.yml\n  - openapi/sap-sd-sales-contract-openapi.yml\n  - openapi/sap-sd-sales-inquiry-openapi.yml\n  - openapi/sap-sd-sales-order-openapi.yml\n  - openapi/sap-sd-sales-quotation-openapi.yml\n  - openapi/sap-sd-sales-scheduling-agreement-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/authentication/sap-sales-and-distribution-sd-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Distribution
- ERP
- OData
- S/4HANA
- Sales
- SAP
---
