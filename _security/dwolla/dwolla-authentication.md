---
api_key_in: []
api_specs:
- filename: dwolla-accounts-openapi.yml
  format: yaml
  label: Dwolla Accounts API
  slug: dwolla-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-accounts-openapi.yml
- filename: dwolla-customers-openapi.yml
  format: yaml
  label: Dwolla Customers API
  slug: dwolla-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-customers-openapi.yml
- filename: dwolla-beneficial-owners-openapi.yml
  format: yaml
  label: Dwolla Beneficial Owners API
  slug: dwolla-beneficial-owners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-beneficial-owners-openapi.yml
- filename: dwolla-kba-openapi.yml
  format: yaml
  label: Dwolla KBA API
  slug: dwolla-kba-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-kba-openapi.yml
- filename: dwolla-documents-openapi.yml
  format: yaml
  label: Dwolla Documents API
  slug: dwolla-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-documents-openapi.yml
- filename: dwolla-funding-sources-openapi.yml
  format: yaml
  label: Dwolla Funding Sources API
  slug: dwolla-funding-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-funding-sources-openapi.yml
- filename: dwolla-transfers-openapi.yml
  format: yaml
  label: Dwolla Transfers API
  slug: dwolla-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-transfers-openapi.yml
- filename: dwolla-mass-payments-openapi.yml
  format: yaml
  label: Dwolla Mass Payments API
  slug: dwolla-mass-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-mass-payments-openapi.yml
- filename: dwolla-labels-openapi.yml
  format: yaml
  label: Dwolla Labels API
  slug: dwolla-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-labels-openapi.yml
- filename: dwolla-exchanges-openapi.yml
  format: yaml
  label: Dwolla Exchanges API
  slug: dwolla-exchanges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-exchanges-openapi.yml
- filename: dwolla-exchange-sessions-openapi.yml
  format: yaml
  label: Dwolla Exchange Sessions API
  slug: dwolla-exchange-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-exchange-sessions-openapi.yml
- filename: dwolla-events-openapi.yml
  format: yaml
  label: Dwolla Events API
  slug: dwolla-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-events-openapi.yml
- filename: dwolla-webhook-subscriptions-openapi.yml
  format: yaml
  label: Dwolla Webhook Subscriptions API
  slug: dwolla-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-webhook-subscriptions-openapi.yml
- filename: dwolla-webhooks-openapi.yml
  format: yaml
  label: Dwolla Webhooks API
  slug: dwolla-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-webhooks-openapi.yml
- filename: dwolla-client-tokens-openapi.yml
  format: yaml
  label: Dwolla Client Tokens API
  slug: dwolla-client-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-client-tokens-openapi.yml
- filename: dwolla-tokens-openapi.yml
  format: yaml
  label: Dwolla Tokens API
  slug: dwolla-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-tokens-openapi.yml
- filename: dwolla-root-openapi.yml
  format: yaml
  label: Dwolla Root API
  slug: dwolla-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-root-openapi.yml
- filename: dwolla-sandbox-simulations-openapi.yml
  format: yaml
  label: Dwolla Sandbox Simulations API
  slug: dwolla-sandbox-simulations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-sandbox-simulations-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Dwolla Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Dwolla secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Dwolla
provider_slug: dwolla
scheme_count: 1
schemes:
- api_request_auth: 'Authorization: Bearer {access_token}'
  description: Application authorization (2-legged OAuth). The application exchanges its client_id and client_secret for an application access token that acts on the app's own behalf.
  flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2ClientCredentials
  token_lifetime: 3600s (one hour); no refresh token — re-exchange credentials on expiry
  token_request_auth: 'HTTP Basic — Authorization: Basic base64(client_id:client_secret)'
  token_urls:
    production: https://api.dwolla.com/token
    sandbox: https://api-sandbox.dwolla.com/token
  type: oauth2
slug: dwolla-authentication
source_filename: dwolla-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developers.dwolla.com/docs/api-reference/api-fundamentals/making-requests-and-authentication\ndocs: https://developers.dwolla.com/docs/api-reference/api-fundamentals/making-requests-and-authentication\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  token_delivery: bearer\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    Application authorization (2-legged OAuth). The application exchanges its client_id and\n    client_secret for an application access token that acts on the app's own behalf.\n  token_urls:\n    production: https://api.dwolla.com/token\n    sandbox: https://api-sandbox.dwolla.com/token\n  grant_type: client_credentials\n  token_request_auth: \"HTTP Basic — Authorization: Basic base64(client_id:client_secret)\"\n  token_lifetime: \"3600s (one hour); no refresh token — re-exchange credentials on expiry\"\n  api_request_auth:\
  \ \"Authorization: Bearer {access_token}\"\nrequest_headers:\n  Accept: application/vnd.dwolla.v1.hal+json\n  Content-Type: application/vnd.dwolla.v1.hal+json (or application/json)\nscopes:\n  note: >-\n    The client-credentials application flow does not use scopes. Scope errors (InvalidScopes) can be\n    returned for endpoints requiring specific granted permissions; a public scope reference was not\n    located, so no scopes/ artifact is emitted (see errors/dwolla-problem-types.yml InvalidScopes).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/authentication/dwolla-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Payments
- ACH
- Bank Transfers
- Fintech
- Account-to-Account Payments
- Money Movement
- Instant Payments
- Open Banking
- Webhooks
- KYC
- United States
- Open Finance
- Same-Day ACH
- RTP
- FedNow
- Mass Payments
- Drop-in Components
- SDKs
- Sandbox
---
