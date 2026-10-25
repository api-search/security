---
anonymous_access: false
api_key_in: []
api_specs:
- filename: basiq-accounts-api-openapi.yml
  format: yaml
  label: Basiq Accounts API
  slug: basiq-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/openapi/basiq-accounts-api-openapi.yml
- filename: basiq-authentication-api-openapi.yml
  format: yaml
  label: Basiq Authentication API
  slug: basiq-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/openapi/basiq-authentication-api-openapi.yml
- filename: basiq-connections-api-openapi.yml
  format: yaml
  label: Basiq Connections API
  slug: basiq-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/openapi/basiq-connections-api-openapi.yml
- filename: basiq-transactions-api-openapi.yml
  format: yaml
  label: Basiq Transactions API
  slug: basiq-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/openapi/basiq-transactions-api-openapi.yml
- filename: basiq-users-api-openapi.yml
  format: yaml
  label: Basiq Users API
  slug: basiq-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/openapi/basiq-users-api-openapi.yml
- filename: basiq-consents-api-openapi.yml
  format: yaml
  label: Basiq Consents API
  slug: basiq-consents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/openapi/basiq-consents-api-openapi.yml
- filename: basiq-jobs-api-openapi.yml
  format: yaml
  label: Basiq Jobs API
  slug: basiq-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/openapi/basiq-jobs-api-openapi.yml
- filename: basiq-affordability-api-openapi.yml
  format: yaml
  label: Basiq Affordability API
  slug: basiq-affordability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/openapi/basiq-affordability-api-openapi.yml
- filename: basiq-analytics-api-openapi.yml
  format: yaml
  label: Basiq Analytics API
  slug: basiq-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/openapi/basiq-analytics-api-openapi.yml
- filename: basiq-authlinks-api-openapi.yml
  format: yaml
  label: Basiq Auth Links API
  slug: basiq-authlinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/openapi/basiq-authlinks-api-openapi.yml
- filename: basiq-connectors-api-openapi.yml
  format: yaml
  label: Basiq Connectors API
  slug: basiq-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/openapi/basiq-connectors-api-openapi.yml
- filename: basiq-enrich-api-openapi.yml
  format: yaml
  label: Basiq Enrich API
  slug: basiq-enrich-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/openapi/basiq-enrich-api-openapi.yml
- filename: basiq-events-api-openapi.yml
  format: yaml
  label: Basiq Events API
  slug: basiq-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/openapi/basiq-events-api-openapi.yml
- filename: basiq-expenses-api-openapi.yml
  format: yaml
  label: Basiq Expenses API
  slug: basiq-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/openapi/basiq-expenses-api-openapi.yml
- filename: basiq-identities-api-openapi.yml
  format: yaml
  label: Basiq Identities API
  slug: basiq-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/openapi/basiq-identities-api-openapi.yml
- filename: basiq-income-api-openapi.yml
  format: yaml
  label: Basiq Income API
  slug: basiq-income-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/openapi/basiq-income-api-openapi.yml
- filename: basiq-insights-api-openapi.yml
  format: yaml
  label: Basiq Insights API
  slug: basiq-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/openapi/basiq-insights-api-openapi.yml
- filename: basiq-payees-api-openapi.yml
  format: yaml
  label: Basiq Payees API
  slug: basiq-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/openapi/basiq-payees-api-openapi.yml
- filename: basiq-reports-api-openapi.yml
  format: yaml
  label: Basiq Reports API
  slug: basiq-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/openapi/basiq-reports-api-openapi.yml
- filename: basiq-statements-api-openapi.yml
  format: yaml
  label: Basiq Statements API
  slug: basiq-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/openapi/basiq-statements-api-openapi.yml
- filename: basiq-webhooks-api-openapi.yml
  format: yaml
  label: Basiq Webhooks API
  slug: basiq-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/openapi/basiq-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Basiq Authentication
name_suffix: Authentication
oauth_flows: []
overview: Basiq secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Basiq
provider_slug: basiq
scheme_count: 2
schemes:
- format: 'Authorization: Basic <your-api-key-as-issued>'
  header: Authorization
  in: header
  name: api_key
  note: '"Unlike standard HTTP Basic Auth, the Basiq API key is passed verbatim as the header value." Base64-encoding the key produces a 400 error.'
  sources:
  - openapi/_original/basiq-openapi.json
  type: apiKey
  used_by:
  - postToken
- name: services_token
  note: Access token from POST /token; "They expire every 60 minutes, so we recommend you store it globally and refresh 2-3 times an hour."
  scheme: bearer
  sources:
  - openapi/_original/basiq-openapi.json
  - openapi/_original/basiq-identity-openapi.json
  - openapi/_original/basiq-webhooks-openapi.json
  token_scopes:
  - description: Server-side token (example value of the token response `scope`).
    name: SERVER_ACCESS
  - description: Client-side token, requested with a userId (example value of the token response `scope`).
    name: CLIENT_ACCESS
  type: http
slug: basiq-authentication
source_filename: basiq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: searched\nsource: https://api.basiq.io/reference/posttoken\ndocs: https://api.basiq.io/reference/posttoken\nsee_also:\n- https://api.basiq.io/docs/api-key-management\n- https://api.basiq.io/docs/getting-started\nsummary:\n  types: [apiKey, http]\n  flow: API key -> POST /token -> bearer access token (expires every 60 minutes)\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  header: Authorization\n  used_by: [postToken]\n  format: 'Authorization: Basic <your-api-key-as-issued>'\n  note: '\"Unlike standard HTTP Basic Auth, the Basiq API key is passed verbatim as the header value.\" Base64-encoding the key produces a 400 error.'\n  sources: [openapi/_original/basiq-openapi.json]\n- name: services_token\n  type: http\n  scheme: bearer\n  note: Access token from POST /token; \"They expire every 60 minutes, so we recommend you store it globally and refresh 2-3 times an hour.\"\n  token_scopes:\n  - name: SERVER_ACCESS\n    description:\
  \ Server-side token (example value of the token response `scope`).\n  - name: CLIENT_ACCESS\n    description: Client-side token, requested with a userId (example value of the token response `scope`).\n  sources: [openapi/_original/basiq-openapi.json, openapi/_original/basiq-identity-openapi.json, openapi/_original/basiq-webhooks-openapi.json]\nheaders:\n- name: basiq-version\n  required: true\n  example: '3.0'\nkey_management:\n  rotation: '\"It is advised that API keys are rotated every 90 days\" (https://api.basiq.io/docs/api-key-management)'\n  issuance: API keys are generated and revoked in the Dashboard 'API Keys' section.\nwebhook_verification:\n  scheme: HMAC-SHA256\n  headers: [webhook-id, webhook-timestamp, webhook-signature]\n  docs: https://api.basiq.io/docs/webhooks-security\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/authentication/basiq-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Australia
- Banking
- CDR
- Financial Data
- Fintech
- Open Banking
- Transaction
- Lending
- Account Verification
---
