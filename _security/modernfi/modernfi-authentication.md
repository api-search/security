---
api_key_in: []
api_specs:
- filename: modernfi-accounts-api-openapi.yml
  format: yaml
  label: ModernFi Accounts API
  slug: modernfi-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modernfi/refs/heads/main/openapi/modernfi-accounts-api-openapi.yml
- filename: modernfi-auth-api-openapi.yml
  format: yaml
  label: ModernFi auth API
  slug: modernfi-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modernfi/refs/heads/main/openapi/modernfi-auth-api-openapi.yml
- filename: modernfi-custombenchmarks-api-openapi.yml
  format: yaml
  label: ModernFi customBenchmarks API
  slug: modernfi-custombenchmarks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modernfi/refs/heads/main/openapi/modernfi-custombenchmarks-api-openapi.yml
- filename: modernfi-depositors-api-openapi.yml
  format: yaml
  label: ModernFi Depositors API
  slug: modernfi-depositors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modernfi/refs/heads/main/openapi/modernfi-depositors-api-openapi.yml
- filename: modernfi-files-api-openapi.yml
  format: yaml
  label: ModernFi files API
  slug: modernfi-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modernfi/refs/heads/main/openapi/modernfi-files-api-openapi.yml
- filename: modernfi-pricinggroups-api-openapi.yml
  format: yaml
  label: ModernFi pricingGroups API
  slug: modernfi-pricinggroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modernfi/refs/heads/main/openapi/modernfi-pricinggroups-api-openapi.yml
- filename: modernfi-transactions-api-openapi.yml
  format: yaml
  label: ModernFi Transactions API
  slug: modernfi-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modernfi/refs/heads/main/openapi/modernfi-transactions-api-openapi.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Modernfi Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: ModernFi secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: ModernFi
provider_slug: modernfi
scheme_count: 2
schemes:
- name: OAuth
  scheme: bearer
  sources:
  - openapi/modernfi-openapi-original.json
  type: http
- access_levels:
  - read-only
  - read+write
  audience: https://api.modernfi.com
  discovery: well-known/modernfi-openid-configuration.json
  flow: clientCredentials
  name: OAuth2ClientCredentials
  source: https://docs.modernfi.com/topics/authentication
  tokenUrl: https://auth.modernfi.com/oauth/token
  type: oauth2
slug: modernfi-authentication
source_filename: modernfi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/modernfi-openapi-original.json\ndocs: https://docs.modernfi.com/topics/authentication\nsummary:\n  types:\n  - oauth2\n  - http\n  oauth2_flows:\n  - clientCredentials\n  identity_provider: Auth0\nnotes: >-\n  The OpenAPI declares a single HTTP bearer scheme named \"OAuth\", but the\n  documented flow is OAuth 2.0 client_credentials. Credentials (Client ID +\n  Client Secret) are issued by ModernFi after institution onboarding and\n  delivered via SendSafely. A token is minted at\n  https://auth.modernfi.com/oauth/token with grant_type=client_credentials and\n  an audience of the target API host, then passed as \"Authorization: Bearer\n  <access_token>\". Access is granted at two coarse levels rather than\n  fine-grained scopes: read-only (retrieve accounts, depositors, transactions,\n  statements) and read+write (full create/modify). Tokens expire in 86400s.\nschemes:\n- name: OAuth\n  type: http\n  scheme: bearer\n\
  \  sources:\n  - openapi/modernfi-openapi-original.json\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://auth.modernfi.com/oauth/token\n  audience: https://api.modernfi.com\n  access_levels:\n  - read-only\n  - read+write\n  source: https://docs.modernfi.com/topics/authentication\n  discovery: well-known/modernfi-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modernfi/refs/heads/main/authentication/modernfi-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Banking
- Deposits
- Fintech
- Credit Unions
- Financial Services
- Deposit Network
- Treasury
---
