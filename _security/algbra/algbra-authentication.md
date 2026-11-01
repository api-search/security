---
anonymous_access: false
api_key_in: []
api_specs:
- filename: algbra-accounts-api-openapi.yml
  format: yaml
  label: Algbra Accounts API
  slug: algbra-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-accounts-api-openapi.yml
- filename: algbra-transactions-api-openapi.yml
  format: yaml
  label: Algbra Transactions API
  slug: algbra-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-transactions-api-openapi.yml
- filename: algbra-automated-payments-api-openapi.yml
  format: yaml
  label: Algbra Automated Payments API
  slug: algbra-automated-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-automated-payments-api-openapi.yml
- filename: algbra-cards-api-openapi.yml
  format: yaml
  label: Algbra Cards API
  slug: algbra-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-cards-api-openapi.yml
- filename: algbra-compliance-api-openapi.yml
  format: yaml
  label: Algbra Compliance API
  slug: algbra-compliance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-compliance-api-openapi.yml
- filename: algbra-customers-api-openapi.yml
  format: yaml
  label: Algbra Customers API
  slug: algbra-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-customers-api-openapi.yml
- filename: algbra-investments-api-openapi.yml
  format: yaml
  label: Algbra Investments API
  slug: algbra-investments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-investments-api-openapi.yml
- filename: algbra-onboarding-prospects-business-api-openapi.yml
  format: yaml
  label: Algbra Onboarding Prospects - Business API
  slug: algbra-onboarding-prospects-business-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-onboarding-prospects-business-api-openapi.yml
- filename: algbra-onboarding-prospects-personal-api-openapi.yml
  format: yaml
  label: Algbra Onboarding Prospects - Personal API
  slug: algbra-onboarding-prospects-personal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-onboarding-prospects-personal-api-openapi.yml
- filename: algbra-partner-api-openapi.yml
  format: yaml
  label: Algbra Partner API
  slug: algbra-partner-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-partner-api-openapi.yml
- filename: algbra-partners-api-openapi.yml
  format: yaml
  label: Algbra Partners API
  slug: algbra-partners-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-partners-api-openapi.yml
- filename: algbra-payment-simulations-api-openapi.yml
  format: yaml
  label: Algbra Payment Simulations API
  slug: algbra-payment-simulations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-payment-simulations-api-openapi.yml
- filename: algbra-payments-api-openapi.yml
  format: yaml
  label: Algbra Payments API
  slug: algbra-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-payments-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Algbra Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Algbra secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Algbra
provider_slug: algbra
scheme_count: 2
schemes:
- description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when a TPP wants to access an ASPSP resource owned by the PSU
  flows:
  - authorizationUrl: https://secure.tell.systems/algbra/auth/oidc/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://secure.tell.systems/algbra/auth/oidc/token
  name: PSUOAuth2Security
  sources:
  - openapi/algbra-account-transaction-api-openapi.yml
  type: oauth2
- description: TPP client credential authorisation flow with the ASPSP
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://secure.tell.systems/algbra/auth/oidc/token
  name: TPPOAuth2Security
  sources:
  - openapi/algbra-account-transaction-api-openapi.yml
  type: oauth2
slug: algbra-authentication
source_filename: algbra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: derived\nsource: openapi/algbra-account-transaction-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: PSUOAuth2Security\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://secure.tell.systems/algbra/auth/oidc/authorize\n    tokenUrl: https://secure.tell.systems/algbra/auth/oidc/token\n    scopes: 1\n  description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when\n    a TPP wants to access an ASPSP resource owned by the PSU\n  sources:\n  - openapi/algbra-account-transaction-api-openapi.yml\n- name: TPPOAuth2Security\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://secure.tell.systems/algbra/auth/oidc/token\n    scopes: 1\n  description: TPP client credential authorisation flow with the ASPSP\n  sources:\n  - openapi/algbra-account-transaction-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/algbra/authentication/algbra-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Financial Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
- Fintech
- Ethical Finance
- Banking as a Service
---
