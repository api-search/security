---
api_key_in:
- header
api_specs:
- filename: highnote-graphql-api-openapi.yml
  format: yaml
  label: Highnote Issuing API
  slug: highnote-issuing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highnote/refs/heads/main/openapi/highnote-graphql-api-openapi.yml
- filename: highnote-graphql-api-openapi.yml
  format: yaml
  label: Highnote Account Holders & Onboarding API
  slug: highnote-account-holders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highnote/refs/heads/main/openapi/highnote-graphql-api-openapi.yml
- filename: highnote-graphql-api-openapi.yml
  format: yaml
  label: Highnote Acquiring API
  slug: highnote-acquiring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highnote/refs/heads/main/openapi/highnote-graphql-api-openapi.yml
- filename: highnote-graphql-api-openapi.yml
  format: yaml
  label: Highnote Money Movement API
  slug: highnote-money-movement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highnote/refs/heads/main/openapi/highnote-graphql-api-openapi.yml
- filename: highnote-graphql-api-openapi.yml
  format: yaml
  label: Highnote Transactions & Disputes API
  slug: highnote-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highnote/refs/heads/main/openapi/highnote-graphql-api-openapi.yml
- filename: highnote-graphql-api-openapi.yml
  format: yaml
  label: Highnote Spend Controls & Collaborative Authorization API
  slug: highnote-spend-controls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highnote/refs/heads/main/openapi/highnote-graphql-api-openapi.yml
- filename: highnote-graphql-api-openapi.yml
  format: yaml
  label: Highnote Webhooks & Event Notifications API
  slug: highnote-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highnote/refs/heads/main/openapi/highnote-graphql-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Highnote Authentication
name_suffix: Authentication
oauth_flows: []
overview: Highnote secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Highnote
provider_slug: highnote
scheme_count: 1
schemes:
- description: 'HTTP Basic auth. Generate an API key in the Highnote Dashboard, base64-encode the ASCII key, and send it as the HTTP Basic username with an empty password — equivalent to `Authorization: Basic <base64(apiKey)>`. Keys are environment-scoped (Test vs Live) and rotatable in the Dashboard. There is no OAuth/OIDC flow.'
  key_management:
    environments:
    - test
    - live
    rotation_docs: https://docs.highnote.com/docs/developers/api/rotating-keys
  name: basicAuth
  scheme: basic
  sources:
  - openapi/highnote-graphql-api-openapi.yml
  type: http
slug: highnote-authentication
source_filename: highnote-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: openapi/highnote-graphql-api-openapi.yml\ndocs: https://docs.highnote.com/docs/developers/api/using-the-api\nsummary:\n  types:\n  - http\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic auth. Generate an API key in the Highnote Dashboard, base64-encode the ASCII key,\n    and send it as the HTTP Basic username with an empty password — equivalent to\n    `Authorization: Basic <base64(apiKey)>`. Keys are environment-scoped (Test vs Live) and\n    rotatable in the Dashboard. There is no OAuth/OIDC flow.\n  key_management:\n    rotation_docs: https://docs.highnote.com/docs/developers/api/rotating-keys\n    environments: [test, live]\n  sources:\n  - openapi/highnote-graphql-api-openapi.yml\nclient_side_auth:\n  detail: Browser/embedded SDK components authenticate with short-lived client tokens minted server-side.\n  docs: https://docs.highnote.com/docs/developers/sdks/client-tokens\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/highnote/refs/heads/main/authentication/highnote-authentication.yml
summary_line: http · 1 scheme
tags:
- Card Issuing
- Card Acquiring
- Embedded Finance
- Banking-as-a-Service
- Fintech
- Payments
- GraphQL
- Ledger
- Credit
- Money Movement
- ACH
- KYC
- United States
---
