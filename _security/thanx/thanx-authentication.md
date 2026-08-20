---
api_key_in:
- header
api_specs:
- filename: thanx-account-api-openapi.yml
  format: yaml
  label: Thanx Account API
  slug: thanx-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-account-api-openapi.yml
- filename: thanx-auth-api-openapi.yml
  format: yaml
  label: Thanx Auth API
  slug: thanx-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-auth-api-openapi.yml
- filename: thanx-baskets-api-openapi.yml
  format: yaml
  label: Thanx Baskets API
  slug: thanx-baskets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-baskets-api-openapi.yml
- filename: thanx-campaigns-api-openapi.yml
  format: yaml
  label: Thanx Campaigns API
  slug: thanx-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-campaigns-api-openapi.yml
- filename: thanx-cards-api-openapi.yml
  format: yaml
  label: Thanx Cards API
  slug: thanx-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-cards-api-openapi.yml
- filename: thanx-gift-cards-api-openapi.yml
  format: yaml
  label: Thanx Gift Cards API
  slug: thanx-gift-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-gift-cards-api-openapi.yml
- filename: thanx-issuance-jobs-api-openapi.yml
  format: yaml
  label: Thanx Issuance Jobs API
  slug: thanx-issuance-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-issuance-jobs-api-openapi.yml
- filename: thanx-locations-api-openapi.yml
  format: yaml
  label: Thanx Locations API
  slug: thanx-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-locations-api-openapi.yml
- filename: thanx-metadata-api-openapi.yml
  format: yaml
  label: Thanx Metadata API
  slug: thanx-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-metadata-api-openapi.yml
- filename: thanx-points-api-openapi.yml
  format: yaml
  label: Thanx Points API
  slug: thanx-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-points-api-openapi.yml
- filename: thanx-purchases-api-openapi.yml
  format: yaml
  label: Thanx Purchases API
  slug: thanx-purchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-purchases-api-openapi.yml
- filename: thanx-rewards-api-openapi.yml
  format: yaml
  label: Thanx Rewards API
  slug: thanx-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-rewards-api-openapi.yml
- filename: thanx-subscribers-api-openapi.yml
  format: yaml
  label: Thanx Subscribers API
  slug: thanx-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-subscribers-api-openapi.yml
- filename: thanx-users-api-openapi.yml
  format: yaml
  label: Thanx Users API
  slug: thanx-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-users-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: Thanx authenticates in three different ways depending on which API family you are calling. Consumer apps carry a user access token minted by Thanx SSO (passwordless OAuth 2.0 authorization code) plus an X-ClientId. Partner server-to-server integrations carry a scope-limited token from POST /partner/oauth/token, also with X-ClientId. The Loyalty (POS/ordering) API on loyalty.thanx.com uses a Merchant-Key instead of X-ClientId, and accepts a Reward-Redemption-Token as an ALTERNATIVE to the user bearer for token-only redemption. No credential is self-serve — all are issued by Thanx, and production credentials only after certification.
kind: authentication
layout: security
method: searched
name: Thanx Authentication
name_suffix: Authentication
oauth_flows: []
overview: Thanx secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Thanx
provider_slug: thanx
scheme_count: 4
schemes:
- applies_to:
  - Consumer
  - Partner
  - Loyalty
  description: End-user access token. On the Consumer and Loyalty APIs it is acquired through Thanx SSO; on the Partner API it is minted at POST /partner/oauth/token.
  header: 'Authorization: Bearer <access_token>'
  name: bearerAuth
  required: Yes, except on the documented unauthenticated endpoints (e.g. GET communication settings by UID) and on Loyalty calls that instead supply a Reward-Redemption-Token.
  scheme: bearer
  sources:
  - https://docs.thanx.com/consumer/usage/headers
  - openapi/*.yml (components.securitySchemes.bearerAuth)
  type: http
- applies_to:
  - Consumer
  - Partner
  description: Client-specific identifier issued by Thanx. Required on every Consumer and Partner request.
  in: header
  name: clientId
  parameter: X-ClientId
  required: true
  sources:
  - https://docs.thanx.com/consumer/usage/headers
  - openapi/*.yml (components.securitySchemes.clientId)
  type: apiKey
- applies_to:
  - Loyalty
  description: Identifies the merchant to the Loyalty API. Issued by Thanx. This replaces X-ClientId on loyalty.thanx.com — sending the Consumer header set to the Loyalty host is a common first-week failure.
  in: header
  name: merchantKey
  parameter: Merchant-Key
  required: true
  sources:
  - https://docs.thanx.com/loyalty/headers
  - openapi/thanx-account-api-openapi.yml
  - openapi/thanx-baskets-api-openapi.yml
  type: apiKey
- applies_to:
  - Loyalty
  description: Token-only redemption credential for the Loyalty basket flow. Send it INSTEAD OF the user Authorization bearer, never alongside it — if both are present the call returns 404 when the merchant lacks indirect loyalty integration, or 401 when the token resolves to no reward.
  in: header
  mutually_exclusive_with: bearerAuth
  name: rewardRedemptionToken
  parameter: Reward-Redemption-Token
  required: false
  sources:
  - https://docs.thanx.com/loyalty/headers
  type: apiKey
slug: thanx-authentication
source_filename: thanx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\ndocs: https://docs.thanx.com/consumer/usage/headers\nsource: >-\n  https://docs.thanx.com/consumer/usage/headers, https://docs.thanx.com/consumer/sso/overview,\n  https://docs.thanx.com/loyalty/headers, https://docs.thanx.com/partner/overview,\n  https://docs.thanx.com/partner/auth/create-token,\n  https://docs.thanx.com/partner/metadata/get-scopes — upgraded from the derived profile\n  (openapi/*.yml securitySchemes), which understated the surface: the specs declare two schemes\n  while Thanx actually runs four distinct credential types across three API families.\ndescription: >-\n  Thanx authenticates in three different ways depending on which API family you are calling.\n  Consumer apps carry a user access token minted by Thanx SSO (passwordless OAuth 2.0\n  authorization code) plus an X-ClientId. Partner server-to-server integrations carry a\n  scope-limited token from POST /partner/oauth/token, also with X-ClientId. The Loyalty\n\
  \  (POS/ordering) API on loyalty.thanx.com uses a Merchant-Key instead of X-ClientId, and accepts\n  a Reward-Redemption-Token as an ALTERNATIVE to the user bearer for token-only redemption.\n  No credential is self-serve — all are issued by Thanx, and production credentials only after\n  certification.\nsummary:\n  types: [apiKey, http, oauth2]\n  api_key_in: [header]\n  oauth2_grants: [authorization_code]\n  self_serve: false\n  mfa_for_api: not applicable\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    header: 'Authorization: Bearer <access_token>'\n    description: >-\n      End-user access token. On the Consumer and Loyalty APIs it is acquired through Thanx SSO;\n      on the Partner API it is minted at POST /partner/oauth/token.\n    applies_to: [Consumer, Partner, Loyalty]\n    required: >-\n      Yes, except on the documented unauthenticated endpoints (e.g. GET communication settings\n      by UID) and on Loyalty calls that instead supply a Reward-Redemption-Token.\n\
  \    sources:\n      - https://docs.thanx.com/consumer/usage/headers\n      - openapi/*.yml (components.securitySchemes.bearerAuth)\n  - name: clientId\n    type: apiKey\n    in: header\n    parameter: X-ClientId\n    description: Client-specific identifier issued by Thanx. Required on every Consumer and Partner request.\n    applies_to: [Consumer, Partner]\n    required: true\n    sources:\n      - https://docs.thanx.com/consumer/usage/headers\n      - openapi/*.yml (components.securitySchemes.clientId)\n  - name: merchantKey\n    type: apiKey\n    in: header\n    parameter: Merchant-Key\n    description: >-\n      Identifies the merchant to the Loyalty API. Issued by Thanx. This replaces X-ClientId on\n      loyalty.thanx.com — sending the Consumer header set to the Loyalty host is a common\n      first-week failure.\n    applies_to: [Loyalty]\n    required: true\n    sources:\n      - https://docs.thanx.com/loyalty/headers\n      - openapi/thanx-account-api-openapi.yml\n      - openapi/thanx-baskets-api-openapi.yml\n\
  \  - name: rewardRedemptionToken\n    type: apiKey\n    in: header\n    parameter: Reward-Redemption-Token\n    description: >-\n      Token-only redemption credential for the Loyalty basket flow. Send it INSTEAD OF the user\n      Authorization bearer, never alongside it — if both are present the call returns 404 when\n      the merchant lacks indirect loyalty integration, or 401 when the token resolves to no\n      reward.\n    applies_to: [Loyalty]\n    required: false\n    mutually_exclusive_with: bearerAuth\n    sources:\n      - https://docs.thanx.com/loyalty/headers\noauth2:\n  spec: RFC 6749 §4.1 (Authorization Code grant)\n  flavor: passwordless — the user is authenticated by an emailed auth link, not a password\n  scope_value: passwordless\n  endpoints:\n    - {name: authorize, path: 'POST /oauth/authorize', note: 'Sends the auth email. Returns 401 when no account exists for the email — create one with POST /users.'}\n    - {name: authorize-cross-domain, path: 'POST /oauth/authorize-cross-domain',\
  \ note: 'Issues an authorization code for an already-authenticated user with no email, for domain-to-domain SSO handoff.'}\n    - {name: token, path: 'POST /oauth/token', note: 'Exchanges the authorization code for an access token.'}\n    - {name: revoke, path: 'POST /oauth/revoke', note: \"Revokes a user's access token.\"}\n  token_response_schema: components.schemas.Authorization (token_type, scope, created_at, access_token, refresh_token)\n  refresh_tokens: true\n  pkce: not documented\n  openid_connect: false\n  discovery: none — /.well-known/openid-configuration and /.well-known/oauth-authorization-server 404 on every host\n  important: >-\n    SSO authenticates a user and issues a token; it does NOT enrol them with the merchant. A\n    user who signs in without a membership receives empty tier and reward responses until\n    POST /users enrols them.\n  docs: https://docs.thanx.com/consumer/sso/overview\npartner_tokens:\n  mint: 'POST /partner/oauth/token (operationId createToken)'\n\
  \  scope_required: auth.create\n  expires_in: optional, 60–3600 seconds\n  scope_model: >-\n    Each credential is provisioned with an agreed-upon set of scopes; endpoints declare the\n    scope they require and return 403 without it. Introspect with GET /partner/scopes.\n  detail: scopes/thanx-scopes.yml\nrequired_headers:\n  consumer_partner:\n    - 'Authorization: Bearer <access_token>'\n    - 'X-ClientId: <client id>'\n    - 'Accept-Version: v4.0'\n    - 'Content-Type: application/json'\n    - 'Accept: application/json'\n  loyalty:\n    - 'Authorization: Bearer <access_token>  # or Reward-Redemption-Token'\n    - 'Merchant-Key: <merchant key>'\n    - 'Accept: application/vnd.thanx-v1+json'\n    - 'Content-Type: application/json'\n    - 'User-Agent: {partner}/1.0.0'\nprovisioning:\n  self_serve: false\n  sandbox: >-\n    Sandbox client id, client secret, merchant key, partner token and a test user are issued by\n    Thanx Developer Support during onboarding (developer.support@thanx.com).\n\
  \  production: >-\n    Released only after a mandatory certification of the integration against the sandbox; each\n    new use-case is re-certified.\n  contacts: {developer: developer.support@thanx.com, partnerships: partnerships@thanx.com}\n  detail: sandbox/thanx-sandbox.yml\ntransport_security:\n  tls: TLS 1.3 on www.thanx.com, docs.thanx.com and api.thanx.com\n  hsts: enabled on all three\n  private_link: AWS PrivateLink available for the Loyalty API (https://docs.thanx.com/loyalty/private-link)\n  pci_hosts: [https://secure.api.thanx.com, https://secure.api.thanxsandbox.com]\n  detail: security/thanx-domain-security.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/authentication/thanx-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Restaurant
- Loyalty
- Guest Engagement
- Marketing
- CRM
- Online Ordering
- Webhook
- Points
- Rewards
- Campaigns
---
