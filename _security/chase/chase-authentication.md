---
api_key_in: []
api_specs:
- filename: chase-account-and-customer-information-api-openapi.yml
  format: yaml
  label: Chase Account and Customer Information API
  slug: account-and-customer-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chase/refs/heads/main/openapi/chase-account-and-customer-information-api-openapi.yml
- filename: chase-account-aggregation-user-consent-api-openapi.yml
  format: yaml
  label: Chase Account Aggregation User Consent API
  slug: account-aggregation-user-consent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chase/refs/heads/main/openapi/chase-account-aggregation-user-consent-api-openapi.yml
- filename: chase-rewards-balance-api-openapi.yml
  format: yaml
  label: Chase Rewards Balance API
  slug: rewards-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chase/refs/heads/main/openapi/chase-rewards-balance-api-openapi.yml
- filename: chase-loyalty-pay-with-points-order-service-api-openapi.yml
  format: yaml
  label: Chase Loyalty Pay with Points Order Service API
  slug: loyalty-pay-with-points-order-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chase/refs/heads/main/openapi/chase-loyalty-pay-with-points-order-service-api-openapi.yml
- filename: chase-loyalty-pay-with-points-enrollment-service-api-openapi.yml
  format: yaml
  label: Chase Loyalty Pay with Points Enrollment Service API
  slug: loyalty-pay-with-points-enrollment-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chase/refs/heads/main/openapi/chase-loyalty-pay-with-points-enrollment-service-api-openapi.yml
- filename: chase-loyalty-pci-merchant-relationship-manager-api-openapi.yml
  format: yaml
  label: Chase Loyalty PCI Merchant Relationship Manager API
  slug: loyalty-pci-merchant-relationship-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chase/refs/heads/main/openapi/chase-loyalty-pci-merchant-relationship-manager-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Chase Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Chase secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Chase
provider_slug: chase
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://api.chase.com/oauth2/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://api.chase.com/oauth2/token
  name: oauth2
  sources:
  - openapi/chase-account-aggregation-user-consent-api-openapi.yml
  - openapi/chase-account-and-customer-information-api-openapi.yml
  type: oauth2
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://api.chase.com/oauth2/token
  name: oauth2
  sources:
  - openapi/chase-loyalty-pay-with-points-enrollment-service-api-openapi.yml
  - openapi/chase-loyalty-pay-with-points-order-service-api-openapi.yml
  - openapi/chase-loyalty-pci-merchant-relationship-manager-api-openapi.yml
  - openapi/chase-rewards-balance-api-openapi.yml
  type: oauth2
slug: chase-authentication
source_filename: chase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/chase-account-aggregation-user-consent-api-openapi.yml, openapi/chase-account-and-customer-information-api-openapi.yml,\n  openapi/chase-loyalty-pay-with-points-enrollment-service-api-openapi.yml, openapi/chase-loyalty-pay-with-points-order-service-api-openapi.yml,\n  openapi/chase-loyalty-pci-merchant-relationship-manager-api-openapi.yml, openapi/chase-rewards-balance-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.chase.com/oauth2/authorize\n    tokenUrl: https://api.chase.com/oauth2/token\n    scopes: 2\n  sources:\n  - openapi/chase-account-aggregation-user-consent-api-openapi.yml\n  - openapi/chase-account-and-customer-information-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.chase.com/oauth2/token\n\
  \    scopes: 1\n  sources:\n  - openapi/chase-loyalty-pay-with-points-enrollment-service-api-openapi.yml\n  - openapi/chase-loyalty-pay-with-points-order-service-api-openapi.yml\n  - openapi/chase-loyalty-pci-merchant-relationship-manager-api-openapi.yml\n  - openapi/chase-rewards-balance-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chase/refs/heads/main/authentication/chase-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Account Aggregation
- Banking
- Consent
- Credit Cards
- FDX
- Financial Services
- Loyalty
- Open Banking
- Pay with Points
- Rewards
---
