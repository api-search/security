---
api_key_in: []
api_specs:
- filename: formance-openapi.yml
  format: yaml
  label: Formance Ledger API
  slug: formance-ledger-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formance/refs/heads/main/openapi/formance-openapi.yml
- filename: formance-openapi.yml
  format: yaml
  label: Formance Payments API
  slug: formance-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formance/refs/heads/main/openapi/formance-openapi.yml
- filename: formance-openapi.yml
  format: yaml
  label: Formance Orchestration API
  slug: formance-orchestration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formance/refs/heads/main/openapi/formance-openapi.yml
- filename: formance-openapi.yml
  format: yaml
  label: Formance Wallets API
  slug: formance-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formance/refs/heads/main/openapi/formance-openapi.yml
- filename: formance-openapi.yml
  format: yaml
  label: Formance Reconciliation API
  slug: formance-reconciliation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formance/refs/heads/main/openapi/formance-openapi.yml
- filename: formance-openapi.yml
  format: yaml
  label: Formance Auth API
  slug: formance-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formance/refs/heads/main/openapi/formance-openapi.yml
- filename: formance-openapi.yml
  format: yaml
  label: Formance Webhooks API
  slug: formance-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formance/refs/heads/main/openapi/formance-openapi.yml
- filename: formance-openapi.yml
  format: yaml
  label: Formance Search API
  slug: formance-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formance/refs/heads/main/openapi/formance-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Formance Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Formance secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Formance
provider_slug: formance
scheme_count: 1
schemes:
- description: 'OAuth2 client-credentials flow. Exchange a client id and secret at `/api/auth/oauth/token` for a Bearer access token, then send it as `Authorization: Bearer <token>`.'
  flows:
  - flow: clientCredentials
    scopes: 6
    tokenUrl: https://{organization}.{environment}.formance.cloud/api/auth/oauth/token
  name: oauth2
  sources:
  - openapi/formance-openapi.yml
  type: oauth2
slug: formance-authentication
source_filename: formance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/formance-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{organization}.{environment}.formance.cloud/api/auth/oauth/token\n    scopes: 6\n  description: 'OAuth2 client-credentials flow. Exchange a client id and secret at `/api/auth/oauth/token`\n    for a Bearer access token, then send it as `Authorization: Bearer <token>`.'\n  sources:\n  - openapi/formance-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/formance/refs/heads/main/authentication/formance-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Financial Infrastructure
- Ledger
- Double-Entry Accounting
- Payments
- Orchestration
- Money Movement
- Open Source
- Fintech
---
