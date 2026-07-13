---
api_key_in:
- header
api_specs:
- filename: overview
  format: yaml
  label: SAP Convergent Charging API
  slug: sap-convergent-charging-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/convergent_charging/overview
- filename: overview
  format: yaml
  label: SAP Convergent Invoicing API
  slug: sap-convergent-invoicing-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/convergent_invoicing/overview
- filename: overview
  format: yaml
  label: SAP Subscription Billing API
  slug: sap-subscription-billing-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/subscription_billing/overview
- filename: overview
  format: yaml
  label: SAP Contract Accounts Receivable and Payable API
  slug: sap-contract-accounts-receivable-and-payable-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/fica/overview
- filename: overview
  format: yaml
  label: SAP BRIM Usage Data Intake API
  slug: sap-brim-usage-data-intake-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/usage_data_intake/overview
- filename: overview
  format: yaml
  label: SAP Revenue Accounting and Reporting API
  slug: sap-revenue-accounting-and-reporting-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/revenue_accounting/overview
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Sap Brim Billing And Revenue Innovation Management Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: SAP BRIM (Billing and Revenue Innovation Management) secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: SAP BRIM (Billing and Revenue Innovation Management)
provider_slug: sap-brim-billing-and-revenue-innovation-management
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://auth.sap.com/oauth/token
  name: OAuth2
  sources:
  - openapi/sap-brim-convergent-charging-openapi.yml
  - openapi/sap-brim-subscription-billing-openapi.yml
  type: oauth2
- in: header
  name: ApiKeyAuth
  parameter: APIKey
  sources:
  - openapi/sap-brim-convergent-charging-openapi.yml
  - openapi/sap-brim-subscription-billing-openapi.yml
  type: apiKey
slug: sap-brim-billing-and-revenue-innovation-management-authentication
source_filename: sap-brim-billing-and-revenue-innovation-management-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sap-brim-convergent-charging-openapi.yml, openapi/sap-brim-subscription-billing-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.sap.com/oauth/token\n    scopes: 2\n  sources:\n  - openapi/sap-brim-convergent-charging-openapi.yml\n  - openapi/sap-brim-subscription-billing-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: APIKey\n  sources:\n  - openapi/sap-brim-convergent-charging-openapi.yml\n  - openapi/sap-brim-subscription-billing-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-brim-billing-and-revenue-innovation-management/refs/heads/main/authentication/sap-brim-billing-and-revenue-innovation-management-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Billing
- Enterprise
- Order to Cash
- Revenue Management
- SAP
- Subscription Management
- Usage-Based Pricing
---
