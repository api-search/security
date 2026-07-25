---
api_key_in: []
api_specs:
- filename: orum-authentication-api-openapi.yml
  format: yaml
  label: Orum Authentication API
  slug: orum-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-authentication-api-openapi.yml
- filename: orum-balance-api-openapi.yml
  format: yaml
  label: Orum Balance API
  slug: orum-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-balance-api-openapi.yml
- filename: orum-book-transfers-api-openapi.yml
  format: yaml
  label: Orum Book Transfers API
  slug: orum-book-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-book-transfers-api-openapi.yml
- filename: orum-businesses-api-openapi.yml
  format: yaml
  label: Orum Businesses API
  slug: orum-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-businesses-api-openapi.yml
- filename: orum-cards-api-openapi.yml
  format: yaml
  label: Orum Cards API
  slug: orum-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-cards-api-openapi.yml
- filename: orum-configure-webhooks-api-openapi.yml
  format: yaml
  label: Orum Configure webhooks API
  slug: orum-configure-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-configure-webhooks-api-openapi.yml
- filename: orum-eligibility-api-openapi.yml
  format: yaml
  label: Orum Eligibility API
  slug: orum-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-eligibility-api-openapi.yml
- filename: orum-external-accounts-api-openapi.yml
  format: yaml
  label: Orum External Accounts API
  slug: orum-external-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-external-accounts-api-openapi.yml
- filename: orum-persons-api-openapi.yml
  format: yaml
  label: Orum Persons API
  slug: orum-persons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-persons-api-openapi.yml
- filename: orum-reports-api-openapi.yml
  format: yaml
  label: Orum Reports API
  slug: orum-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-reports-api-openapi.yml
- filename: orum-schedules-api-openapi.yml
  format: yaml
  label: Orum Schedules API
  slug: orum-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-schedules-api-openapi.yml
- filename: orum-secure-webhooks-api-openapi.yml
  format: yaml
  label: Orum Secure webhooks API
  slug: orum-secure-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-secure-webhooks-api-openapi.yml
- filename: orum-subledgers-api-openapi.yml
  format: yaml
  label: Orum Subledgers API
  slug: orum-subledgers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-subledgers-api-openapi.yml
- filename: orum-transfer-groups-api-openapi.yml
  format: yaml
  label: Orum Transfer Groups API
  slug: orum-transfer-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-transfer-groups-api-openapi.yml
- filename: orum-transfers-api-openapi.yml
  format: yaml
  label: Orum Transfers API
  slug: orum-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-transfers-api-openapi.yml
- filename: orum-trigger-webhooks-api-openapi.yml
  format: yaml
  label: Orum Trigger webhooks API
  slug: orum-trigger-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-trigger-webhooks-api-openapi.yml
- filename: orum-verify-api-openapi.yml
  format: yaml
  label: Orum Verify API
  slug: orum-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-verify-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Orum Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Orum secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Orum
provider_slug: orum
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 29
    tokenUrl: https://api-sandbox.orum.io/oauth/token
  name: oauth2
  sources:
  - openapi/orum-openapi-original.yml
  type: oauth2
slug: orum-authentication
source_filename: orum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/orum-openapi-original.yml\ndocs: https://docs.orum.io/guides/api-authentication\nnotes: >-\n  OAuth 2.0 client-credentials. Create client_id/client_secret in Monitor\n  (Developer Tools -> API Authentication); max two credential sets per Enterprise\n  per environment. Exchange at /oauth/token for a bearer access token; the secret\n  is shown only once. Rotate by generating a new set before deleting the old.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-sandbox.orum.io/oauth/token\n    scopes: 29\n  sources:\n  - openapi/orum-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/authentication/orum-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Payments
- Fintech
- Banking
- Instant Payments
- ACH
- Money Movement
- Bank Account Verification
---
