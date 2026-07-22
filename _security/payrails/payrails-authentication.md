---
api_key_in: []
auth_types:
- oauth2
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Payrails Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Payrails secures its APIs with oauth2 and mutualTLS across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Payrails
provider_slug: payrails
scheme_count: 3
schemes:
- applied_as: Authorization bearer token on all API calls
  flow: clientCredentials
  name: OAuth2ClientCredentials
  request: POST with Client ID (path) + Client Secret credential
  response_field: access token with expires_in
  source: https://docs.payrails.com/reference/getoauthtoken
  token_lifetime_seconds: 3600
  token_url: https://api.payrails.io/auth/token/{clientId}
  token_url_staging: https://api.staging.payrails.io/auth/token/{clientId}
  type: oauth2
- docs: https://docs.payrails.com/docs/mtls-configuration-1
  name: mTLS
  notes: Mutual TLS client-certificate connection option for backend integrations.
  type: mutualTLS
- algorithm: HMAC-SHA256
  docs: https://docs.payrails.com/docs/receive-notifications
  encoding: base64
  header: X-Signature
  name: WebhookHMAC
  notes: Notifications carry an X-Signature header (base64 HMAC-SHA256 of the payload using a portal-generated secret) so receivers can verify authenticity. This secures inbound webhooks, not outbound API auth.
  scope: inbound-notifications
  type: hmac
slug: payrails-authentication
source_filename: payrails-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.payrails.com/reference/getoauthtoken\ndocs: https://docs.payrails.com/docs/api-credentials-1\nsummary:\n  types: [oauth2, mutualTLS]\n  oauth2_flows: [clientCredentials]\n  notes: >-\n    Backend services exchange a Client ID + Client Secret (scoped per environment)\n    for a short-lived bearer access token, then call Payrails APIs with that token.\n    Access tokens are valid for one hour and must be refreshed on expiry. mTLS is\n    additionally available to secure the connection to Payrails. Credentials are\n    created and scoped per environment (Staging vs Production) in the Payrails Portal.\nschemes:\n  - name: OAuth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    token_url: https://api.payrails.io/auth/token/{clientId}\n    token_url_staging: https://api.staging.payrails.io/auth/token/{clientId}\n    token_lifetime_seconds: 3600\n    request: POST with Client ID (path) + Client Secret\
  \ credential\n    response_field: access token with expires_in\n    applied_as: Authorization bearer token on all API calls\n    source: https://docs.payrails.com/reference/getoauthtoken\n  - name: mTLS\n    type: mutualTLS\n    docs: https://docs.payrails.com/docs/mtls-configuration-1\n    notes: Mutual TLS client-certificate connection option for backend integrations.\n  - name: WebhookHMAC\n    type: hmac\n    scope: inbound-notifications\n    algorithm: HMAC-SHA256\n    header: X-Signature\n    encoding: base64\n    docs: https://docs.payrails.com/docs/receive-notifications\n    notes: >-\n      Notifications carry an X-Signature header (base64 HMAC-SHA256 of the payload\n      using a portal-generated secret) so receivers can verify authenticity. This\n      secures inbound webhooks, not outbound API auth.\nroles_permissions:\n  model: RBAC (roles & permissions assigned per API service / workspace)\n  docs: https://docs.payrails.com/docs/roles-permissions\nsso:\n  saml: true\n  docs:\
  \ https://docs.payrails.com/docs/single-sign-on\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payrails/refs/heads/main/authentication/payrails-authentication.yml
summary_line: oauth2/mutualTLS · 3 schemes
tags:
- Company
- Payments
- Payment Orchestration
- Fintech
- Tokenization
- Fraud
- Disputes
- Reconciliation
- Checkout
- Financial Infrastructure
---
