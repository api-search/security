---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Astra Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Astra secures its APIs with oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Astra
provider_slug: astra
scheme_count: 3
schemes:
- authorization_url: https://app.astra.finance/login/oauth/authorize
  description: Authorization Code flow. Present the user with Astra's OAuth module, receive an authorization_code, then exchange it at the token endpoint for a Bearer access_token used on that user's API requests.
  flow: authorizationCode
  name: OAuth2 (user authorization)
  source: https://docs.astra.finance/reference/authorization
  token_endpoint: https://api.astra.finance/v1/oauth/token
  type: oauth2
- description: Client-level authorization using the application's client_id and client_secret for administrative endpoints that are not scoped to a single end user.
  flow: clientCredentials
  name: Client Credentials (administrative)
  source: https://docs.astra.finance/docs/api-only-authorization
  type: oauth2
- description: Enterprise onboarding variant for personal users offering the most onboarding flexibility, built on the same OAuth authorization model.
  name: Trusted Authentication
  source: https://docs.astra.finance/docs/trusted-authentication
  type: oauth2
slug: astra-authentication
source_filename: astra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.astra.finance/reference/authorization\ndocs: https://docs.astra.finance/reference/authorization\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode, clientCredentials]\n  transport: https-only\n  token_header: \"Authorization: Bearer <access_token>\"\nnotes: >-\n  All API requests must be made over HTTPS; plain HTTP and unauthenticated\n  requests fail. End-user money-movement operations are authorized with an\n  OAuth 2.0 access_token obtained by exchanging a temporary authorization_code;\n  administrative/client-level operations use client credentials\n  (client_id/client_secret issued from the Developer Dashboard). Astra also\n  documents \"Trusted Authentication\" and \"API Only Authorization\" onboarding\n  variants layered on the same OAuth model.\nschemes:\n- name: OAuth2 (user authorization)\n  type: oauth2\n  description: >-\n    Authorization Code flow. Present the user with Astra's OAuth\
  \ module, receive\n    an authorization_code, then exchange it at the token endpoint for a Bearer\n    access_token used on that user's API requests.\n  flow: authorizationCode\n  token_endpoint: https://api.astra.finance/v1/oauth/token\n  authorization_url: https://app.astra.finance/login/oauth/authorize\n  source: https://docs.astra.finance/reference/authorization\n- name: Client Credentials (administrative)\n  type: oauth2\n  description: >-\n    Client-level authorization using the application's client_id and\n    client_secret for administrative endpoints that are not scoped to a single\n    end user.\n  flow: clientCredentials\n  source: https://docs.astra.finance/docs/api-only-authorization\n- name: Trusted Authentication\n  type: oauth2\n  description: >-\n    Enterprise onboarding variant for personal users offering the most\n    onboarding flexibility, built on the same OAuth authorization model.\n  source: https://docs.astra.finance/docs/trusted-authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/astra/refs/heads/main/authentication/astra-authentication.yml
summary_line: oauth2 · 3 schemes
tags:
- Company
- Payments
- Fintech
- Money Movement
- ACH
- Instant Payments
- Bank Transfers
- Disbursements
- API
---
