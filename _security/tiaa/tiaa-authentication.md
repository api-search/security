---
api_key_in: []
api_specs:
- filename: tiaa-accounts-api-openapi.yml
  format: yaml
  label: TIAA Accounts API
  slug: tiaa-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiaa/refs/heads/main/openapi/tiaa-accounts-api-openapi.yml
- filename: tiaa-contributions-api-openapi.yml
  format: yaml
  label: TIAA Contributions API
  slug: tiaa-contributions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiaa/refs/heads/main/openapi/tiaa-contributions-api-openapi.yml
- filename: tiaa-customer-api-openapi.yml
  format: yaml
  label: TIAA Customer API
  slug: tiaa-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiaa/refs/heads/main/openapi/tiaa-customer-api-openapi.yml
- filename: tiaa-investments-api-openapi.yml
  format: yaml
  label: TIAA Investments API
  slug: tiaa-investments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiaa/refs/heads/main/openapi/tiaa-investments-api-openapi.yml
- filename: tiaa-participants-api-openapi.yml
  format: yaml
  label: TIAA Participants API
  slug: tiaa-participants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiaa/refs/heads/main/openapi/tiaa-participants-api-openapi.yml
- filename: tiaa-plans-api-openapi.yml
  format: yaml
  label: TIAA Plans API
  slug: tiaa-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiaa/refs/heads/main/openapi/tiaa-plans-api-openapi.yml
- filename: tiaa-projections-api-openapi.yml
  format: yaml
  label: TIAA Projections API
  slug: tiaa-projections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiaa/refs/heads/main/openapi/tiaa-projections-api-openapi.yml
- filename: tiaa-tax-api-openapi.yml
  format: yaml
  label: TIAA Tax API
  slug: tiaa-tax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiaa/refs/heads/main/openapi/tiaa-tax-api-openapi.yml
- filename: tiaa-transactions-api-openapi.yml
  format: yaml
  label: TIAA Transactions API
  slug: tiaa-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiaa/refs/heads/main/openapi/tiaa-transactions-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Tiaa Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: TIAA secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: TIAA
provider_slug: tiaa
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://auth.tiaa.org/oauth2/authorize
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://auth.tiaa.org/oauth2/token
  name: OAuth2
  sources:
  - openapi/tiaa-fdx-openapi.yml
  type: oauth2
- flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://auth.tiaa.org/oauth2/token
  name: ClientCredentials
  sources:
  - openapi/tiaa-sia-openapi.yml
  type: oauth2
slug: tiaa-authentication
source_filename: tiaa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tiaa-fdx-openapi.yml, openapi/tiaa-sia-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.tiaa.org/oauth2/authorize\n    tokenUrl: https://auth.tiaa.org/oauth2/token\n    scopes: 6\n  sources:\n  - openapi/tiaa-fdx-openapi.yml\n- name: ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.tiaa.org/oauth2/token\n    scopes: 2\n  sources:\n  - openapi/tiaa-sia-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tiaa/refs/heads/main/authentication/tiaa-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Finance
- Financial Data
- Fintech
- Insurance
- Investment Management
- Retirement
- Wealth Management
- Fortune 100
---
