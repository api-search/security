---
api_key_in: []
auth_types:
- oauth2
- http
description: Hotmart Developers authenticates every API call with OAuth 2.0. Credentials (client_id, client_secret and a pre-computed Basic token) are minted in the Hotmart platform under Tools > Developer Credentials, and are bound at creation time to either the production or the sandbox environment — the type cannot be changed afterwards, a new credential must be created. The credential is exchanged for a short-lived access_token at the token endpoint, which is then sent as a Bearer token on every resource request.
kind: authentication
layout: security
method: searched
name: Hotmart Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Hotmart secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Hotmart
provider_slug: hotmart
scheme_count: 2
schemes:
- client_authentication: HTTP Basic — the "Basic" token generated alongside client_id/client_secret is sent in the Authorization header on the token request; client_id and client_secret are additionally passed as query parameters.
  flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2ClientCredentials
  request_example: 'POST https://api-sec-vlc.hotmart.com/security/oauth/token?grant_type=client_credentials&client_id=:client_id&client_secret=:client_secret with headers Content-Type: application/json and Authorization: Basic :basic'
  scopes_documented: false
  scopes_note: Hotmart does not publish an OAuth scope/permission reference. Access is determined by the Hotmart account (and collaborator permissions) the credential belongs to, not by requested scopes, so no scopes/ artifact is emitted.
  sources:
  - https://developers.hotmart.com/docs/en/start/app-auth/
  token_url: https://api-sec-vlc.hotmart.com/security/oauth/token
  type: oauth2
- description: 'The access_token returned by the token endpoint is sent on every resource request as `Authorization: Bearer <access_token>`.'
  name: BearerToken
  scheme: bearer
  sources:
  - https://developers.hotmart.com/docs/en/start/app-auth/
  type: http
slug: hotmart-authentication
source_filename: hotmart-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://developers.hotmart.com/docs/en/start/app-auth/\ndocs: https://developers.hotmart.com/docs/en/start/app-auth/\ndescription: >-\n  Hotmart Developers authenticates every API call with OAuth 2.0. Credentials\n  (client_id, client_secret and a pre-computed Basic token) are minted in the\n  Hotmart platform under Tools > Developer Credentials, and are bound at creation\n  time to either the production or the sandbox environment — the type cannot be\n  changed afterwards, a new credential must be created. The credential is\n  exchanged for a short-lived access_token at the token endpoint, which is then\n  sent as a Bearer token on every resource request.\nsummary:\n  types: [oauth2, http]\n  api_key_in: []\n  oauth2_flows: [clientCredentials]\n  bearer_on_requests: true\nschemes:\n  - name: OAuth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    token_url: https://api-sec-vlc.hotmart.com/security/oauth/token\n\
  \    grant_type: client_credentials\n    client_authentication: >-\n      HTTP Basic — the \"Basic\" token generated alongside client_id/client_secret\n      is sent in the Authorization header on the token request; client_id and\n      client_secret are additionally passed as query parameters.\n    request_example: >-\n      POST https://api-sec-vlc.hotmart.com/security/oauth/token?grant_type=client_credentials&client_id=:client_id&client_secret=:client_secret\n      with headers Content-Type: application/json and Authorization: Basic :basic\n    scopes_documented: false\n    scopes_note: >-\n      Hotmart does not publish an OAuth scope/permission reference. Access is\n      determined by the Hotmart account (and collaborator permissions) the\n      credential belongs to, not by requested scopes, so no scopes/ artifact is\n      emitted.\n    sources: [https://developers.hotmart.com/docs/en/start/app-auth/]\n  - name: BearerToken\n    type: http\n    scheme: bearer\n    description:\
  \ >-\n      The access_token returned by the token endpoint is sent on every resource\n      request as `Authorization: Bearer <access_token>`.\n    sources: [https://developers.hotmart.com/docs/en/start/app-auth/]\ntoken:\n  response_fields: [access_token, token_type, expires_in, scope, jti]\n  expiry_field: expires_in\n  expiry_note: >-\n    expires_in indicates the time allotted before the token expires; after that\n    period every request made with the same token returns 401. Hotmart\n    recommends the application handle the 401 and re-run token generation. Only\n    the access token expires — client_id, client_secret and the Basic token do\n    not rotate on their own.\n  error_on_expiry:\n    http_status: 401\n    error_types: [token_expired, invalid_token, unauthorized]\nenvironments:\n  - name: production\n    credential_type: production\n    token_url: https://api-sec-vlc.hotmart.com/security/oauth/token\n    api_host: https://developers.hotmart.com\n  - name: sandbox\n    credential_type:\
  \ sandbox\n    token_url: https://api-sec-vlc.hotmart.com/security/oauth/token\n    api_host: https://sandbox.hotmart.com\n    note: >-\n      Sandbox requires a credential created with the \"sandbox\" type checked; a\n      production credential will not authenticate against sandbox.hotmart.com.\ncredential_management:\n  console: https://app-vlc.hotmart.com/tools/credentials\n  path: Hotmart platform > Tools > Developer Credentials\n  rotation: >-\n    Credentials can be deleted and regenerated at any time from the credentials\n    tool if exposure is suspected.\nwebhook_authentication:\n  mechanism: shared secret (\"hottok\")\n  header: X-HOTMART-HOTTOK\n  description: >-\n    Every webhook delivery carries the account's unique hottok in the\n    X-HOTMART-HOTTOK HTTP header. Hotmart recommends validating it before\n    processing the payload. It is a static per-account shared secret, not a\n    signature — there is no HMAC body signature or timestamp/replay defence\n    documented.\n\
  \  rotation: by Hotmart support request only\n  docs: https://developers.hotmart.com/docs/en/2.0.0/webhook/purchase-webhook/\nx-evidence:\n  fetched: '2026-08-04'\n  urls:\n    - https://developers.hotmart.com/docs/en/start/app-auth/\n    - https://developers.hotmart.com/docs/en/start/sandbox/\n    - https://developers.hotmart.com/docs/en/2.0.0/webhook/purchase-webhook/\n  probe:\n    - url: https://api-sec-vlc.hotmart.com/security/oauth/token\n      method: POST\n      http_status: 401\n      note: unauthenticated probe — endpoint is live and rejects anonymous callers\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hotmart/refs/heads/main/authentication/hotmart-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Creator Economy
- Digital Products
- Online Courses
- E-Commerce
- Payments
- Subscription
- Affiliate Marketing
- Webhook
- Learning Management
- Brazil
---
