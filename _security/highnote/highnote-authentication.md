---
api_key_in: []
api_specs:
- filename: highnote-openapi.yml
  format: yaml
  label: Highnote Card Issuing API
  slug: card-issuing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highnote/refs/heads/main/openapi/highnote-openapi.yml
- filename: highnote-openapi.yml
  format: yaml
  label: Highnote Account Holders API
  slug: account-holders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highnote/refs/heads/main/openapi/highnote-openapi.yml
- filename: highnote-openapi.yml
  format: yaml
  label: Highnote Financial Accounts API
  slug: financial-accounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highnote/refs/heads/main/openapi/highnote-openapi.yml
- filename: highnote-openapi.yml
  format: yaml
  label: Highnote Transactions API
  slug: transactions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highnote/refs/heads/main/openapi/highnote-openapi.yml
- filename: highnote-openapi.yml
  format: yaml
  label: Highnote Transfers API
  slug: transfers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highnote/refs/heads/main/openapi/highnote-openapi.yml
- filename: highnote-openapi.yml
  format: yaml
  label: Highnote Collaborative Authorization API
  slug: collaborative-authorization
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highnote/refs/heads/main/openapi/highnote-openapi.yml
- filename: highnote-openapi.yml
  format: yaml
  label: Highnote Webhooks & Notifications API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highnote/refs/heads/main/openapi/highnote-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Highnote Authentication
name_suffix: Authentication
oauth_flows: []
overview: Highnote secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Highnote
provider_slug: highnote
scheme_count: 1
schemes:
- description: 'HTTP Basic auth. The base64-encoded API key is supplied as the username and the password is left empty. Equivalent to sending `Authorization: Basic <base64(apiKey)>`.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/highnote-openapi.yml
  type: http
slug: highnote-authentication
source_filename: highnote-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/highnote-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'HTTP Basic auth. The base64-encoded API key is supplied as the username and\n    the password is left empty. Equivalent to sending `Authorization: Basic <base64(apiKey)>`.'\n  sources:\n  - openapi/highnote-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/highnote/refs/heads/main/authentication/highnote-authentication.yml
summary_line: http · 1 scheme
tags:
- Card Issuing
- Embedded Finance
- Fintech
- Payments
- GraphQL
- Ledger
- Credit
---
