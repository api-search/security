---
api_key_in: []
api_specs:
- filename: lendkey-application-contracts-api-openapi.yml
  format: yaml
  label: LendKey Application Contracts API
  slug: lendkey-application-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-application-contracts-api-openapi.yml
- filename: lendkey-applications-api-openapi.yml
  format: yaml
  label: LendKey applications API
  slug: lendkey-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-applications-api-openapi.yml
- filename: lendkey-auth-api-openapi.yml
  format: yaml
  label: LendKey auth API
  slug: lendkey-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-auth-api-openapi.yml
- filename: lendkey-authentication-api-openapi.yml
  format: yaml
  label: LendKey Authentication API
  slug: lendkey-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-authentication-api-openapi.yml
- filename: lendkey-credit-risk-api-openapi.yml
  format: yaml
  label: LendKey Credit Risk API
  slug: lendkey-credit-risk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-credit-risk-api-openapi.yml
- filename: lendkey-disbursements-api-openapi.yml
  format: yaml
  label: LendKey Disbursements API
  slug: lendkey-disbursements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-disbursements-api-openapi.yml
- filename: lendkey-email-api-openapi.yml
  format: yaml
  label: LendKey email API
  slug: lendkey-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-email-api-openapi.yml
- filename: lendkey-internal-api-openapi.yml
  format: yaml
  label: LendKey internal API
  slug: lendkey-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-internal-api-openapi.yml
- filename: lendkey-leads-api-openapi.yml
  format: yaml
  label: LendKey leads API
  slug: lendkey-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-leads-api-openapi.yml
- filename: lendkey-ledger-management-api-openapi.yml
  format: yaml
  label: LendKey Ledger Management API
  slug: lendkey-ledger-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-ledger-management-api-openapi.yml
- filename: lendkey-lender-templates-api-openapi.yml
  format: yaml
  label: LendKey Lender Templates API
  slug: lendkey-lender-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-lender-templates-api-openapi.yml
- filename: lendkey-loans-api-openapi.yml
  format: yaml
  label: LendKey Loans API
  slug: lendkey-loans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-loans-api-openapi.yml
- filename: lendkey-onboarding-api-openapi.yml
  format: yaml
  label: LendKey onboarding API
  slug: lendkey-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-onboarding-api-openapi.yml
- filename: lendkey-payments-api-openapi.yml
  format: yaml
  label: LendKey Payments API
  slug: lendkey-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-payments-api-openapi.yml
- filename: lendkey-webhooks-api-openapi.yml
  format: yaml
  label: LendKey Webhooks API
  slug: lendkey-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-webhooks-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Lendkey Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: LendKey secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: LendKey
provider_slug: lendkey
scheme_count: 1
schemes:
- description: OAuth2 client credentials flow via Kong Gateway
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: /oauth2/token
  name: oauth2
  sources:
  - openapi/lendkey-esign-openapi.yml
  - openapi/lendkey-partner-integration-internal-openapi.yml
  - openapi/lendkey-treasury-management-openapi.yml
  type: oauth2
slug: lendkey-authentication
source_filename: lendkey-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/lendkey-esign-openapi.yml, openapi/lendkey-partner-integration-internal-openapi.yml,\n  openapi/lendkey-treasury-management-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/token\n    scopes: 0\n  description: OAuth2 client credentials flow via Kong Gateway\n  sources:\n  - openapi/lendkey-esign-openapi.yml\n  - openapi/lendkey-partner-integration-internal-openapi.yml\n  - openapi/lendkey-treasury-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/authentication/lendkey-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Fintech
- Lending
- Loans
- Student Loans
- Credit Unions
- Banking
- Loan Origination
- Financial-Services
- Payments
- E-Signature
- Treasury
---
