---
api_key_in: []
auth_types:
- oauth1
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Morgan Stanley Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Morgan Stanley secures its APIs with oauth1 and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Morgan Stanley
provider_slug: morgan-stanley
scheme_count: 2
schemes:
- consumer_key: Per-application consumer key + secret; separate keys for sandbox vs production.
  flow:
  - method: GET
    note: Temporary request token, expires after 5 minutes. Requires oauth_consumer_key, oauth_timestamp (epoch, within 5 min), oauth_nonce, oauth_signature_method=HMAC-SHA1, oauth_signature, oauth_callback=oob.
    sandbox_url: https://apisb.etrade.com/oauth/request_token
    step: request_token
    url: https://api.etrade.com/oauth/request_token
  - method: GET
    note: User authorizes the application and receives a verification code.
    step: authorize
    url: https://us.etrade.com/e/t/etws/authorize
  - method: GET
    note: Exchanges the authorized request token + verifier for an access token/secret.
    sandbox_url: https://apisb.etrade.com/oauth/access_token
    step: access_token
    url: https://api.etrade.com/oauth/access_token
  - method: GET
    note: Reactivates an access token that has become inactive (2h idle timeout).
    step: renew_access_token
    url: https://api.etrade.com/oauth/renew_access_token
  - method: GET
    note: Invalidates the access token.
    step: revoke_access_token
    url: https://api.etrade.com/oauth/revoke_access_token
  legs: 3
  name: etrade-oauth1
  signature_method: HMAC-SHA1
  sources:
  - https://apisb.etrade.com/docs/api/authorization/request_token.html
  surface: E*TRADE from Morgan Stanley (Accounts, Market Data, Order, Alerts)
  token_lifetime: Access token is invalidated at midnight US Eastern and becomes inactive after 2 hours of inactivity (renewable via renew_access_token).
  type: oauth1
  version: 1.0a
- credential: Certificate-based confidential-client authentication - client id, tenant, scopes, certificate thumbprint, and a self-signed private key (no shared client secret). Tokens acquired via the MSAL library.
  flow: clientCredentials
  gated: true
  identity_provider: Microsoft Entra / Azure AD (confidential client)
  name: morgan-stanley-platform-oauth2
  scopes: Provisioned per client during onboarding; not published publicly.
  sources:
  - https://github.com/morganstanley/api
  surface: Morgan Stanley API Platform (institutional REST + WebSocket)
  type: oauth2
slug: morgan-stanley-authentication
source_filename: morgan-stanley-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://apisb.etrade.com/docs/api/authorization/request_token.html\ndocs:\n  - https://developer.etrade.com/getting-started\n  - https://apisb.etrade.com/docs/api/authorization/request_token.html\n  - https://github.com/morganstanley/api\nsummary:\n  types: [oauth1, oauth2]\n  api_key_in: []\n  oauth2_flows: [clientCredentials]\n  note: >-\n    Two distinct auth models. The public E*TRADE brokerage API uses three-legged\n    OAuth 1.0a (HMAC-SHA1) on behalf of an account holder. The invitation-only\n    Morgan Stanley institutional API Platform uses OAuth 2.0 confidential-client\n    credentials against Microsoft Entra / Azure AD with certificate-based token\n    exchange (no client secret; a self-signed key pair + certificate thumbprint\n    via the MSAL library). No apiKey/bearer static-key surface is published.\nschemes:\n  - name: etrade-oauth1\n    surface: E*TRADE from Morgan Stanley (Accounts, Market Data, Order, Alerts)\n\
  \    type: oauth1\n    version: 1.0a\n    signature_method: HMAC-SHA1\n    legs: 3\n    flow:\n      - step: request_token\n        method: GET\n        url: https://api.etrade.com/oauth/request_token\n        sandbox_url: https://apisb.etrade.com/oauth/request_token\n        note: >-\n          Temporary request token, expires after 5 minutes. Requires\n          oauth_consumer_key, oauth_timestamp (epoch, within 5 min), oauth_nonce,\n          oauth_signature_method=HMAC-SHA1, oauth_signature, oauth_callback=oob.\n      - step: authorize\n        method: GET\n        url: https://us.etrade.com/e/t/etws/authorize\n        note: User authorizes the application and receives a verification code.\n      - step: access_token\n        method: GET\n        url: https://api.etrade.com/oauth/access_token\n        sandbox_url: https://apisb.etrade.com/oauth/access_token\n        note: Exchanges the authorized request token + verifier for an access token/secret.\n      - step: renew_access_token\n\
  \        method: GET\n        url: https://api.etrade.com/oauth/renew_access_token\n        note: Reactivates an access token that has become inactive (2h idle timeout).\n      - step: revoke_access_token\n        method: GET\n        url: https://api.etrade.com/oauth/revoke_access_token\n        note: Invalidates the access token.\n    token_lifetime: >-\n      Access token is invalidated at midnight US Eastern and becomes inactive after\n      2 hours of inactivity (renewable via renew_access_token).\n    consumer_key: Per-application consumer key + secret; separate keys for sandbox vs production.\n    sources: [https://apisb.etrade.com/docs/api/authorization/request_token.html]\n  - name: morgan-stanley-platform-oauth2\n    surface: Morgan Stanley API Platform (institutional REST + WebSocket)\n    type: oauth2\n    flow: clientCredentials\n    identity_provider: Microsoft Entra / Azure AD (confidential client)\n    credential: >-\n      Certificate-based confidential-client authentication\
  \ - client id, tenant,\n      scopes, certificate thumbprint, and a self-signed private key (no shared\n      client secret). Tokens acquired via the MSAL library.\n    scopes: Provisioned per client during onboarding; not published publicly.\n    gated: true\n    sources: [https://github.com/morganstanley/api]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/morgan-stanley/refs/heads/main/authentication/morgan-stanley-authentication.yml
summary_line: oauth1/oauth2 · 2 schemes
tags:
- Financial
- Investment Banking
- Wealth Management
- Brokerage
- Market Data
- Trading
- Fortune 100
- United States
---
