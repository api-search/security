---
api_key_in: []
api_specs:
- filename: lendkey-integration-openapi.yml
  format: yaml
  label: LendKey Integration API
  slug: integration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-integration-openapi.yml
- filename: lendkey-treasury-management-openapi.yml
  format: yaml
  label: LendKey Treasury Management API
  slug: treasury-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-treasury-management-openapi.yml
- filename: lendkey-esign-openapi.yml
  format: yaml
  label: LendKey E-Sign API
  slug: esign
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-esign-openapi.yml
- filename: lendkey-partner-integration-internal-openapi.yml
  format: yaml
  label: LendKey Partner Integration Internal API
  slug: partner-integration-internal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-partner-integration-internal-openapi.yml
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
- Financial Services
- Payments
- E-Signature
- Treasury
---
