---
api_key_in:
- header
- query
api_specs:
- filename: awin-affiliate-accounts-api-openapi.yml
  format: yaml
  label: Awin Accounts API
  slug: awin-affiliate-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/awin-affiliate/refs/heads/main/openapi/awin-affiliate-accounts-api-openapi.yml
- filename: awin-affiliate-commission-groups-api-openapi.yml
  format: yaml
  label: Awin Commission Groups API
  slug: awin-affiliate-commission-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/awin-affiliate/refs/heads/main/openapi/awin-affiliate-commission-groups-api-openapi.yml
- filename: awin-affiliate-programmes-api-openapi.yml
  format: yaml
  label: Awin Programmes API
  slug: awin-affiliate-programmes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/awin-affiliate/refs/heads/main/openapi/awin-affiliate-programmes-api-openapi.yml
- filename: awin-affiliate-reports-api-openapi.yml
  format: yaml
  label: Awin Reports API
  slug: awin-affiliate-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/awin-affiliate/refs/heads/main/openapi/awin-affiliate-reports-api-openapi.yml
- filename: awin-affiliate-transactions-api-openapi.yml
  format: yaml
  label: Awin Transactions API
  slug: awin-affiliate-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/awin-affiliate/refs/heads/main/openapi/awin-affiliate-transactions-api-openapi.yml
auth_types:
- http
- apiKey
description: 'Awin authenticates with a single long-lived token bound to a USER, not to an account and not to an application. The token is created by a human in the platform UI at https://ui.awin.com/awin-api after re-entering their password, and it grants access to every publisher and advertiser account that user can reach - Awin states this explicitly: "If you have access to 10 different Awin publisher accounts via our website, then your personal API token grants you access to data from all of those 10 accounts." Awin describes this as OAuth 2.0, but only bearer-token presentation (RFC 6750) is implemented: there is no authorization endpoint, no token endpoint, no client registration, no grant flow, no refresh and no scopes.'
kind: authentication
layout: security
method: searched
name: Awin Affiliate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Awin secures its APIs with http and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Awin
provider_slug: awin-affiliate
scheme_count: 3
schemes:
- description: 'Default for every Awin API except Create Transactions / Conversion API. Example from the docs - curl -X GET https://api.awin.com/publishers -H "Authorization: Bearer <token>".'
  format: Bearer <token>
  in: header
  name: bearerAuth
  parameter: Authorization
  scheme: bearer
  sources:
  - https://help.awin.com/apidocs/api-authentication
  - openapi/_original/awin-affiliate-openapi.yml
  type: http
- applies_to:
  - https://help.awin.com/apidocs/conversion-api
  description: Used ONLY by the Create Transactions / Conversion API (POST https://api.awin.com/s2s/advertiser/{advertiser_id}/orders). The same token value is sent bare, without the "Bearer" prefix.
  in: header
  name: apiKeyHeader
  parameter: x-api-key
  sources:
  - https://help.awin.com/apidocs/api-authentication
  type: apiKey
- description: Many GET endpoints additionally accept the token as an `accessToken` query parameter, and the API reference lists it as Required on several endpoints (e.g. Get Link Builder Quota). Documented, but a credential-in-URL pattern that leaks into server logs, proxy logs, referrers and browser history.
  in: query
  name: accessTokenQuery
  parameter: accessToken
  sources:
  - https://help.awin.com/apidocs/quota
  - openapi/_original/awin-affiliate-openapi.yml
  type: apiKey
slug: awin-affiliate-authentication
source_filename: awin-affiliate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://help.awin.com/apidocs/api-authentication\ndocs: https://help.awin.com/apidocs/api-authentication\ndescription: >-\n  Awin authenticates with a single long-lived token bound to a USER, not to an\n  account and not to an application. The token is created by a human in the\n  platform UI at https://ui.awin.com/awin-api after re-entering their password,\n  and it grants access to every publisher and advertiser account that user can\n  reach - Awin states this explicitly: \"If you have access to 10 different Awin\n  publisher accounts via our website, then your personal API token grants you\n  access to data from all of those 10 accounts.\" Awin describes this as OAuth\n  2.0, but only bearer-token presentation (RFC 6750) is implemented: there is no\n  authorization endpoint, no token endpoint, no client registration, no grant\n  flow, no refresh and no scopes.\nsummary:\n  types:\n  - http\n  - apiKey\n  api_key_in:\n \
  \ - header\n  - query\n  oauth2_flows: []\n  scopes: none\n  token_lifetime: non-expiring until manually revoked\n  token_granularity: user\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  format: \"Bearer <token>\"\n  description: >-\n    Default for every Awin API except Create Transactions / Conversion API.\n    Example from the docs - curl -X GET https://api.awin.com/publishers -H\n    \"Authorization: Bearer <token>\".\n  sources:\n  - https://help.awin.com/apidocs/api-authentication\n  - openapi/_original/awin-affiliate-openapi.yml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: >-\n    Used ONLY by the Create Transactions / Conversion API (POST\n    https://api.awin.com/s2s/advertiser/{advertiser_id}/orders). The same token\n    value is sent bare, without the \"Bearer\" prefix.\n  applies_to:\n  - https://help.awin.com/apidocs/conversion-api\n  sources:\n  - https://help.awin.com/apidocs/api-authentication\n\
  - name: accessTokenQuery\n  type: apiKey\n  in: query\n  parameter: accessToken\n  description: >-\n    Many GET endpoints additionally accept the token as an `accessToken` query\n    parameter, and the API reference lists it as Required on several endpoints\n    (e.g. Get Link Builder Quota). Documented, but a credential-in-URL pattern\n    that leaks into server logs, proxy logs, referrers and browser history.\n  sources:\n  - https://help.awin.com/apidocs/quota\n  - openapi/_original/awin-affiliate-openapi.yml\ntoken_issuance:\n  url: https://ui.awin.com/awin-api\n  ui_path: User menu (top right) > API Credentials\n  requires: Admin access on the account, plus re-entry of the account password\n  permission_path:\n    advertisers: Account > Account Permissions\n    publishers: Account > User Permissions\n  propagation_delay: >-\n    Adding or removing a user from an account can take up to 10 minutes to take\n    effect on the token's reach.\n  programmatic: false\ntoken_revocation:\n\
  \  url: https://ui.awin.com/awin-api\n  method: '\"Revoke my API token\" button in the UI'\n  effect: >-\n    Immediate and total - every integration using that token stops working at\n    once. There is no per-integration credential to rotate independently.\n  programmatic: false\nentitlement:\n  note: >-\n    Advertiser API access is gated by commercial plan - \"API access for\n    Advertisers is limited to Accelerate and Advanced plans only.\" Publisher API\n    access is not plan-gated. See plans/awin-affiliate-plans-pricing.yml.\ngaps:\n- No OAuth authorization-code or client-credentials flow; no application identity.\n- No scopes - a token that only needs to read reports can also validate transactions and create offers.\n- No expiry and no rotation story; the only lifecycle event is manual revocation.\n- No per-account or per-integration credentials - blast radius is every account the human can reach.\n- No /.well-known/openid-configuration or /.well-known/oauth-authorization-server\
  \ (both 404 on all hosts).\n- No MFA/step-up documented for token creation beyond password re-entry.\nx-evidence:\n  fetched: '2026-08-13'\n  probes:\n  - url: https://help.awin.com/apidocs/api-authentication.md\n    http_status: 200\n  - url: https://api.awin.com/.well-known/openid-configuration\n    http_status: 404\n  - url: https://api.awin.com/.well-known/oauth-authorization-server\n    http_status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/awin-affiliate/refs/heads/main/authentication/awin-affiliate-authentication.yml
summary_line: http/apiKey · 3 schemes
tags:
- Affiliate Marketing
- Advertising
- Publishers
- Advertisers
- Transaction
- Reporting
- Commissions
- Performance Marketing
---
