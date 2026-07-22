---
api_key_in: []
api_specs:
- filename: lean-technologies-account-on-file-openapi.yml
  format: yaml
  label: Lean UAE Open Finance & Payments
  slug: lean-uae-open-finance-payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-technologies/refs/heads/main/openapi/lean-technologies-account-on-file-openapi.yml
- filename: lean-technologies-ksa-accounts-access-consents-openapi.yml
  format: yaml
  label: Lean KSA Open Banking
  slug: lean-ksa-open-banking
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-technologies/refs/heads/main/openapi/lean-technologies-ksa-accounts-access-consents-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Lean Technologies Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Lean Technologies secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Lean Technologies
provider_slug: lean-technologies
scheme_count: 2
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/lean-technologies-account-on-file-openapi.yml
  - openapi/lean-technologies-bank-data-openapi.yml
  - openapi/lean-technologies-banks-openapi.yml
  - openapi/lean-technologies-consents-openapi.yml
  - openapi/lean-technologies-core-resources-openapi.yml
  - openapi/lean-technologies-customers-openapi.yml
  - openapi/lean-technologies-data-openapi.yml
  - openapi/lean-technologies-enrichment-openapi.yml
  - openapi/lean-technologies-entities-openapi.yml
  - openapi/lean-technologies-files-openapi.yml
  - openapi/lean-technologies-insights-openapi.yml
  - openapi/lean-technologies-ksa-accounts-access-consents-openapi.yml
  - openapi/lean-technologies-ksa-bank-data-openapi.yml
  - openapi/lean-technologies-ksa-core-resources-openapi.yml
  - openapi/lean-technologies-ksa-customers-openapi.yml
  - openapi/lean-technologies-ksa-enrichment-openapi.yml
  - openapi/lean-technologies-ksa-insights-openapi.yml
  - openapi/lean-technologies-ksa-open-banking-openapi.yml
  - openapi/lean-technologies-ksa-payouts-openapi.yml
  - openapi/lean-technologies-ksa-reports-openapi.yml
  - openapi/lean-technologies-ksa-verifications-openapi.yml
  - openapi/lean-technologies-payment-links-openapi.yml
  - openapi/lean-technologies-payments-core-openapi.yml
  - openapi/lean-technologies-payments-customers-openapi.yml
  - openapi/lean-technologies-payments-openapi.yml
  - openapi/lean-technologies-payouts-extended-openapi.yml
  - openapi/lean-technologies-payouts-openapi.yml
  - openapi/lean-technologies-reconciliation-extended-openapi.yml
  - openapi/lean-technologies-reconciliation-openapi.yml
  - openapi/lean-technologies-refunds-openapi.yml
  - openapi/lean-technologies-schedules-openapi.yml
  - openapi/lean-technologies-sessions-openapi.yml
  - openapi/lean-technologies-verifications-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: /auth/token
  name: OAuth2
  sources:
  - openapi/lean-technologies-payment-links-openapi.yml
  - openapi/lean-technologies-schedules-openapi.yml
  - openapi/lean-technologies-sessions-openapi.yml
  type: oauth2
slug: lean-technologies-authentication
source_filename: lean-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\ndocs: https://docs.leantech.me/docs/authentication\nauthorization_server: https://auth.leantech.me\ntoken_endpoint: https://auth.leantech.me/oauth2/token\nsandbox_token_endpoint: https://auth.sandbox.leantech.me/oauth2/token\nfapi_features: [PAR, DPoP, mTLS-client-auth, certificate-bound-tokens, token-exchange, device-code, PKCE-S256]\nscopes_documented: [api, \"customer.<customer_id>\"]\nsource: openapi/lean-technologies-account-on-file-openapi.yml, openapi/lean-technologies-bank-data-openapi.yml,\n  openapi/lean-technologies-banks-openapi.yml, openapi/lean-technologies-consents-openapi.yml,\n  openapi/lean-technologies-core-resources-openapi.yml, openapi/lean-technologies-customers-openapi.yml,\n  openapi/lean-technologies-data-openapi.yml, openapi/lean-technologies-enrichment-openapi.yml,\n  openapi/lean-technologies-entities-openapi.yml, openapi/lean-technologies-files-openapi.yml,\n  openapi/lean-technologies-insights-openapi.yml,\
  \ openapi/lean-technologies-ksa-accounts-access-consents-openapi.yml\n  ...\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/lean-technologies-account-on-file-openapi.yml\n  - openapi/lean-technologies-bank-data-openapi.yml\n  - openapi/lean-technologies-banks-openapi.yml\n  - openapi/lean-technologies-consents-openapi.yml\n  - openapi/lean-technologies-core-resources-openapi.yml\n  - openapi/lean-technologies-customers-openapi.yml\n  - openapi/lean-technologies-data-openapi.yml\n  - openapi/lean-technologies-enrichment-openapi.yml\n  - openapi/lean-technologies-entities-openapi.yml\n  - openapi/lean-technologies-files-openapi.yml\n  - openapi/lean-technologies-insights-openapi.yml\n  - openapi/lean-technologies-ksa-accounts-access-consents-openapi.yml\n  - openapi/lean-technologies-ksa-bank-data-openapi.yml\n  - openapi/lean-technologies-ksa-core-resources-openapi.yml\n\
  \  - openapi/lean-technologies-ksa-customers-openapi.yml\n  - openapi/lean-technologies-ksa-enrichment-openapi.yml\n  - openapi/lean-technologies-ksa-insights-openapi.yml\n  - openapi/lean-technologies-ksa-open-banking-openapi.yml\n  - openapi/lean-technologies-ksa-payouts-openapi.yml\n  - openapi/lean-technologies-ksa-reports-openapi.yml\n  - openapi/lean-technologies-ksa-verifications-openapi.yml\n  - openapi/lean-technologies-payment-links-openapi.yml\n  - openapi/lean-technologies-payments-core-openapi.yml\n  - openapi/lean-technologies-payments-customers-openapi.yml\n  - openapi/lean-technologies-payments-openapi.yml\n  - openapi/lean-technologies-payouts-extended-openapi.yml\n  - openapi/lean-technologies-payouts-openapi.yml\n  - openapi/lean-technologies-reconciliation-extended-openapi.yml\n  - openapi/lean-technologies-reconciliation-openapi.yml\n  - openapi/lean-technologies-refunds-openapi.yml\n  - openapi/lean-technologies-schedules-openapi.yml\n  - openapi/lean-technologies-sessions-openapi.yml\n\
  \  - openapi/lean-technologies-verifications-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /auth/token\n    scopes: 1\n  sources:\n  - openapi/lean-technologies-payment-links-openapi.yml\n  - openapi/lean-technologies-schedules-openapi.yml\n  - openapi/lean-technologies-sessions-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lean-technologies/refs/heads/main/authentication/lean-technologies-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Open Banking
- Open Finance
- Payments
- Financial Data
- Fintech
- MENA
- UAE
- Saudi Arabia
- Pay by Bank
- Bank Data
- Account Verification
- Payouts
---
