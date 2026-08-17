---
api_key_in:
- header
api_specs:
- filename: push-cendyn-crm-openapi.yml
  format: yaml
  label: Cendyn CRM (PUSHTech) REST API
  slug: cendyn-crm-pushtech-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/openapi/push-cendyn-crm-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Push Authentication
name_suffix: Authentication
oauth_flows: []
overview: Push secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Push
provider_slug: push
scheme_count: 1
schemes:
- description: Token authentication. The account secret (or account master secret) is passed in the Authorization header after the literal string "Token token=". The docs' worked example uses the base64-looking string dGVzdEBleGFtcGxlLmNvbTpsZXRtZWlu, which decodes to "test@example.com:letmein" — a documentation placeholder, not a live credential.
  format: Token token={{account_secret}}
  header_name: Authorization
  id: accountToken
  in: header
  sources:
  - https://developers.cendyncrm.com/api/authentication
  - openapi/push-cendyn-crm-openapi.yml
  type: apiKey
  variants:
  - credential: account_secret
    description: Account-level authentication for account-scoped resources (the default on all 67 documented operations).
    header: 'Authorization: Token token={{account_secret}}'
    name: account
  - credential: account_master_secret
    description: Elevated account credential. The reference shows it on the Sync Data resource and on the delivery-send examples; the docs do not state which operations require it, so an integrator must read each operation's Headers block.
    header: 'Authorization: Token token={{account_master_secret}}'
    name: account-master
  - credential: app_secret
    description: App-level authentication. Each app registered in the account has its own secret. Used by the Web SDK (new PUSHTechSDK(app_id, app_secret, user_id)) rather than by the REST API operations documented in the reference.
    name: apps
slug: push-authentication
source_filename: push-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developers.cendyncrm.com/api/authentication\nsuperseded_source: http://developers.pushtech.com/api/authentication\nsuperseded_note: >-\n  The host this artifact was originally read from, developers.pushtech.com, no longer resolves\n  (NXDOMAIN as of 2026-08-13). The developer portal moved to developers.cendyncrm.com following\n  the PUSHTech to Cendyn CRM rebrand; the API host's own 404 body points there.\napi: Cendyn CRM (PUSHTech) REST API\nbase_urls:\n- {url: 'https://api.eu.cendyncrm.com', region: EU}\n- {url: 'https://api.us.cendyncrm.com', region: US}\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- id: accountToken\n  type: apiKey\n  in: header\n  header_name: Authorization\n  format: 'Token token={{account_secret}}'\n  sources:\n  - https://developers.cendyncrm.com/api/authentication\n  - openapi/push-cendyn-crm-openapi.yml\n\
  \  description: >-\n    Token authentication. The account secret (or account master secret) is passed in the\n    Authorization header after the literal string \"Token token=\". The docs' worked example uses\n    the base64-looking string dGVzdEBleGFtcGxlLmNvbTpsZXRtZWlu, which decodes to\n    \"test@example.com:letmein\" — a documentation placeholder, not a live credential.\n  variants:\n  - name: account\n    credential: account_secret\n    header: 'Authorization: Token token={{account_secret}}'\n    description: Account-level authentication for account-scoped resources (the default on all 67 documented operations).\n  - name: account-master\n    credential: account_master_secret\n    header: 'Authorization: Token token={{account_master_secret}}'\n    description: >-\n      Elevated account credential. The reference shows it on the Sync Data resource and on the\n      delivery-send examples; the docs do not state which operations require it, so an integrator\n      must read each operation's\
  \ Headers block.\n  - name: apps\n    credential: app_secret\n    description: >-\n      App-level authentication. Each app registered in the account has its own secret. Used by\n      the Web SDK (new PUSHTechSDK(app_id, app_secret, user_id)) rather than by the REST API\n      operations documented in the reference.\noauth2: false\nscopes:\n  published: false\n  note: >-\n    No OAuth2 flow, token endpoint, refresh contract, scope vocabulary or permission model is\n    published. Authorization is all-or-nothing on the account secret, with the master secret as\n    the only privilege distinction. scopes/ is deliberately not emitted for this provider.\ncredential_management:\n  rotation_policy: not documented\n  expiry: not documented\n  self_serve_issuance: >-\n    Account and app secrets are read from the Cendyn CRM manager UI (apps section, View App\n    details). No API exists to mint, rotate or revoke a credential.\nobserved:\n  method: probed\n  date: '2026-08-13'\n  url: https://api.eu.cendyncrm.com/v2/account/000000000000000000000000/contact\n\
  \  http_status: 401\n  body: '{\"error\":\"authorization failure for account: 000000000000000000000000\"}'\n  www_authenticate: absent\n  note: >-\n    A missing or invalid token returns 401 with the flat {\"error\": ...} envelope and NO\n    WWW-Authenticate challenge header, so the auth scheme is not machine-discoverable from a\n    failed request.\nnotes: >-\n  Single-scheme, header-borne static token. Two credential tiers (account secret, account master\n  secret) plus a separate per-app secret used by the Web SDK. No OAuth2, no OIDC, no mTLS, no\n  scopes, and no published rotation or expiry policy.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/authentication/push-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- CRM
- Customer Data Platform
- Marketing Automation
- Hospitality
- Hotels
- Guest Experience
- Email
- SMS
- Push Notifications
- Webhooks
- Segmentation
---
