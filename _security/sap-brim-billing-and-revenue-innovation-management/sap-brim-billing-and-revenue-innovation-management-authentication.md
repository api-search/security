---
api_key_in:
- header
api_specs:
- filename: sap-brim-billing-and-revenue-innovation-management-balances-api-openapi.yml
  format: yaml
  label: SAP BRIM (Billing and Revenue Innovation Management) Balances API
  slug: sap-brim-billing-and-revenue-innovation-management-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-brim-billing-and-revenue-innovation-management/refs/heads/main/openapi/sap-brim-billing-and-revenue-innovation-management-balances-api-openapi.yml
- filename: sap-brim-billing-and-revenue-innovation-management-billing-api-openapi.yml
  format: yaml
  label: SAP BRIM (Billing and Revenue Innovation Management) Billing API
  slug: sap-brim-billing-and-revenue-innovation-management-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-brim-billing-and-revenue-innovation-management/refs/heads/main/openapi/sap-brim-billing-and-revenue-innovation-management-billing-api-openapi.yml
- filename: sap-brim-billing-and-revenue-innovation-management-charging-api-openapi.yml
  format: yaml
  label: SAP BRIM (Billing and Revenue Innovation Management) Charging API
  slug: sap-brim-billing-and-revenue-innovation-management-charging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-brim-billing-and-revenue-innovation-management/refs/heads/main/openapi/sap-brim-billing-and-revenue-innovation-management-charging-api-openapi.yml
- filename: sap-brim-billing-and-revenue-innovation-management-customers-api-openapi.yml
  format: yaml
  label: SAP BRIM (Billing and Revenue Innovation Management) Customers API
  slug: sap-brim-billing-and-revenue-innovation-management-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-brim-billing-and-revenue-innovation-management/refs/heads/main/openapi/sap-brim-billing-and-revenue-innovation-management-customers-api-openapi.yml
- filename: sap-brim-billing-and-revenue-innovation-management-plans-api-openapi.yml
  format: yaml
  label: SAP BRIM (Billing and Revenue Innovation Management) Plans API
  slug: sap-brim-billing-and-revenue-innovation-management-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-brim-billing-and-revenue-innovation-management/refs/heads/main/openapi/sap-brim-billing-and-revenue-innovation-management-plans-api-openapi.yml
- filename: sap-brim-billing-and-revenue-innovation-management-pricing-api-openapi.yml
  format: yaml
  label: SAP BRIM (Billing and Revenue Innovation Management) Pricing API
  slug: sap-brim-billing-and-revenue-innovation-management-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-brim-billing-and-revenue-innovation-management/refs/heads/main/openapi/sap-brim-billing-and-revenue-innovation-management-pricing-api-openapi.yml
- filename: sap-brim-billing-and-revenue-innovation-management-rating-api-openapi.yml
  format: yaml
  label: SAP BRIM (Billing and Revenue Innovation Management) Rating API
  slug: sap-brim-billing-and-revenue-innovation-management-rating-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-brim-billing-and-revenue-innovation-management/refs/heads/main/openapi/sap-brim-billing-and-revenue-innovation-management-rating-api-openapi.yml
- filename: sap-brim-billing-and-revenue-innovation-management-subscription-items-api-openapi.yml
  format: yaml
  label: SAP BRIM (Billing and Revenue Innovation Management) Subscription Items API
  slug: sap-brim-billing-and-revenue-innovation-management-subscription-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-brim-billing-and-revenue-innovation-management/refs/heads/main/openapi/sap-brim-billing-and-revenue-innovation-management-subscription-items-api-openapi.yml
- filename: sap-brim-billing-and-revenue-innovation-management-subscriptions-api-openapi.yml
  format: yaml
  label: SAP BRIM (Billing and Revenue Innovation Management) Subscriptions API
  slug: sap-brim-billing-and-revenue-innovation-management-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-brim-billing-and-revenue-innovation-management/refs/heads/main/openapi/sap-brim-billing-and-revenue-innovation-management-subscriptions-api-openapi.yml
- filename: sap-brim-billing-and-revenue-innovation-management-usage-events-api-openapi.yml
  format: yaml
  label: SAP BRIM (Billing and Revenue Innovation Management) Usage Events API
  slug: sap-brim-billing-and-revenue-innovation-management-usage-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-brim-billing-and-revenue-innovation-management/refs/heads/main/openapi/sap-brim-billing-and-revenue-innovation-management-usage-events-api-openapi.yml
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
