---
api_key_in:
- body
auth_types:
- apiKey
- custom-token
description: ''
kind: authentication
layout: security
method: searched
name: Levelup Authentication
name_suffix: Authentication
oauth_flows: []
overview: LevelUp secures its APIs with apiKey and custom-token across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LevelUp
provider_slug: levelup
scheme_count: 4
schemes:
- audience: application / point-of-sale integration
  format: token <app_access_token>
  header: Authorization
  in: header
  name: appAccessToken
  obtained_by: POST access_tokens with api_key (app API key) + client_secret; returns an app access token.
  type: custom-token
- audience: merchant account
  format: token merchant="<merchant_access_token>"
  header: Authorization
  in: header
  name: merchantAccessToken
  obtained_by: POST access_tokens with the merchant account username + password (plus the app API key).
  type: custom-token
  v14_format: token <merchant_access_token>
- audience: end user / consumer account
  format: token user="<user_access_token>"
  header: Authorization
  in: header
  name: userAccessToken
  type: custom-token
- audience: combined merchant + user context
  format: token merchant="<merchant_access_token>", user="<user_access_token>"
  header: Authorization
  in: header
  name: merchantAndUserAccessToken
  type: custom-token
slug: levelup-authentication
source_filename: levelup-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  https://github.com/TheLevelUp/levelup-sdk-ruby (lib/levelup/requests/base.rb,\n  lib/levelup/endpoints/access_tokens.rb, README), https://github.com/TheLevelUp/levelup-sdk-csharp (README)\ndocs: null\ndocs_note: >-\n  The canonical auth documentation lived at http://developer.thelevelup.com/api-reference/ ,\n  which no longer resolves. The profile below is reconstructed verbatim from the first-party\n  open-source SDKs, which are the surviving authoritative description of the auth model.\nstatus: retired\nsummary:\n  types: [apiKey, custom-token]\n  api_key_in: [body]\n  token_in: [header]\n  token_header: Authorization\n  token_scheme: token\n  oauth2_flows: []\n  note: >-\n    LevelUp used a bearer-like access-token model with a custom \"token\" Authorization scheme\n    rather than OAuth 2.0. Credentials (app API key + client secret, or merchant username +\n    password) were exchanged at the access_tokens endpoint\
  \ for an access token, which was then\n    sent on the Authorization header. There is no OAuth 2.0 scope surface, so no scopes/ artifact.\nschemes:\n- name: appAccessToken\n  type: custom-token\n  in: header\n  header: Authorization\n  format: 'token <app_access_token>'\n  obtained_by: >-\n    POST access_tokens with api_key (app API key) + client_secret; returns an app access token.\n  audience: application / point-of-sale integration\n- name: merchantAccessToken\n  type: custom-token\n  in: header\n  header: Authorization\n  format: 'token merchant=\"<merchant_access_token>\"'\n  v14_format: 'token <merchant_access_token>'\n  obtained_by: >-\n    POST access_tokens with the merchant account username + password (plus the app API key).\n  audience: merchant account\n- name: userAccessToken\n  type: custom-token\n  in: header\n  header: Authorization\n  format: 'token user=\"<user_access_token>\"'\n  audience: end user / consumer account\n- name: merchantAndUserAccessToken\n  type: custom-token\n\
  \  in: header\n  header: Authorization\n  format: 'token merchant=\"<merchant_access_token>\", user=\"<user_access_token>\"'\n  audience: combined merchant + user context\nauth_types_in_sdk:\n  enumerated: [none, merchant, app, merchant_and_user, user, merchant_v14]\n  source: levelup-sdk-ruby lib/levelup/requests/base.rb auth_header_value\ntransport_requirements:\n- requirement: TLS 1.2 required\n  scope: [www.thelevelup.com, api.thelevelup.com]\n  reason: PCI security standards compliance\n  source: https://github.com/TheLevelUp/levelup-sdk-csharp\n  tooling: https://github.com/TheLevelUp/pos-tls-patcher\nenvironments:\n- {name: sandbox, base_url: 'https://sandbox.thelevelup.com/', real_money: false, dns: NXDOMAIN}\n- {name: production, base_url: 'https://api.thelevelup.com/', real_money: true, dns: NXDOMAIN}\n- {name: staging, base_url: null, note: 'referenced as a built-in LevelUpEnvironment in the C# SDK'}\nsignup: 'https://www.thelevelup.com/users/new (now redirects to grubhub.com)'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/levelup/refs/heads/main/authentication/levelup-authentication.yml
summary_line: apiKey/custom-token · 4 schemes
tags:
- Company
- Consumer
- Payments
- Mobile Payments
- Point of Sale
- Loyalty
- Restaurants
- Retired
---
