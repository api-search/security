---
api_key_in:
- query
api_specs:
- filename: stannp-account-api-openapi.yml
  format: yaml
  label: Stannp Account API
  slug: stannp-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stannp/refs/heads/main/openapi/stannp-account-api-openapi.yml
- filename: stannp-campaigns-api-openapi.yml
  format: yaml
  label: Stannp Campaigns API
  slug: stannp-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stannp/refs/heads/main/openapi/stannp-campaigns-api-openapi.yml
- filename: stannp-events-api-openapi.yml
  format: yaml
  label: Stannp Events API
  slug: stannp-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stannp/refs/heads/main/openapi/stannp-events-api-openapi.yml
- filename: stannp-groups-api-openapi.yml
  format: yaml
  label: Stannp Groups API
  slug: stannp-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stannp/refs/heads/main/openapi/stannp-groups-api-openapi.yml
- filename: stannp-letters-api-openapi.yml
  format: yaml
  label: Stannp Letters API
  slug: stannp-letters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stannp/refs/heads/main/openapi/stannp-letters-api-openapi.yml
- filename: stannp-postcards-api-openapi.yml
  format: yaml
  label: Stannp Postcards API
  slug: stannp-postcards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stannp/refs/heads/main/openapi/stannp-postcards-api-openapi.yml
- filename: stannp-recipients-api-openapi.yml
  format: yaml
  label: Stannp Recipients API
  slug: stannp-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stannp/refs/heads/main/openapi/stannp-recipients-api-openapi.yml
auth_types:
- http
- apiKey
description: Every Stannp API call is authenticated with one account-level API key. The key can be presented two ways — as the HTTP Basic username with an empty password, or as an `api_key` query parameter — and both grant the same full account access. There are no scopes, no per-key permissions, no token exchange, no refresh and no documented rotation or revocation endpoint; keys are managed in the account settings UI. Upgraded from `derived` because the OpenAPI in this repo captures only the HTTP Basic form, while Stannp documents both.
kind: authentication
layout: security
method: searched
name: Stannp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stannp secures its APIs with http and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Stannp
provider_slug: stannp
scheme_count: 3
schemes:
- description: 'Send the API key as the HTTP Basic username with an empty password: `curl "https://api-us1.stannp.com/v1/accounts/balance" -u {API_KEY}:`'
  documented: true
  in_spec: true
  name: basicAuth
  scheme: basic
  sources:
  - openapi/stannp-account-api-openapi.yml
  - openapi/stannp-campaigns-api-openapi.yml
  - openapi/stannp-events-api-openapi.yml
  - openapi/stannp-groups-api-openapi.yml
  - openapi/stannp-letters-api-openapi.yml
  - openapi/stannp-postcards-api-openapi.yml
  - openapi/stannp-recipients-api-openapi.yml
  type: http
- description: Append `?api_key={API_KEY}` to the request URL. Documented by Stannp but NOT declared in any OpenAPI in this repo.
  documented: true
  in: query
  in_spec: false
  name: apiKeyQuery
  parameter_name: api_key
  risk_note: A key in the query string is logged by proxies, CDNs, browser history and server access logs. HTTP Basic is the safer of the two published options.
  source: https://www.stannp.com/us/direct-mail-api/guide
  type: apiKey
- description: QR-code generation takes a PUBLIC key rather than the private API key, because the resulting image URL is embedded in mail artwork and rendered by third parties.
  documented: true
  in: query
  in_spec: false
  name: publicKey
  parameter_name: api_key
  scope: /v1/qrcode/create only
  source: https://www.stannp.com/us/direct-mail-api/tools
  type: apiKey
slug: stannp-authentication
source_filename: stannp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://www.stannp.com/us/direct-mail-api/guide\ndocs: https://www.stannp.com/us/direct-mail-api/guide\nderived_from:\n  - openapi/stannp-account-api-openapi.yml\n  - openapi/stannp-campaigns-api-openapi.yml\n  - openapi/stannp-events-api-openapi.yml\n  - openapi/stannp-groups-api-openapi.yml\n  - openapi/stannp-letters-api-openapi.yml\n  - openapi/stannp-postcards-api-openapi.yml\n  - openapi/stannp-recipients-api-openapi.yml\nsummary:\n  types:\n    - http\n    - apiKey\n  http_schemes:\n    - basic\n  api_key_in:\n    - query\n  oauth2_flows: []\n  model: single static account API key, no scopes, no expiry, no rotation API\ndescription: >-\n  Every Stannp API call is authenticated with one account-level API key. The key\n  can be presented two ways — as the HTTP Basic username with an empty password,\n  or as an `api_key` query parameter — and both grant the same full account\n  access. There are no scopes, no per-key permissions,\
  \ no token exchange, no\n  refresh and no documented rotation or revocation endpoint; keys are managed in\n  the account settings UI. Upgraded from `derived` because the OpenAPI in this\n  repo captures only the HTTP Basic form, while Stannp documents both.\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    description: >-\n      Send the API key as the HTTP Basic username with an empty password:\n      `curl \"https://api-us1.stannp.com/v1/accounts/balance\" -u {API_KEY}:`\n    documented: true\n    in_spec: true\n    sources:\n      - openapi/stannp-account-api-openapi.yml\n      - openapi/stannp-campaigns-api-openapi.yml\n      - openapi/stannp-events-api-openapi.yml\n      - openapi/stannp-groups-api-openapi.yml\n      - openapi/stannp-letters-api-openapi.yml\n      - openapi/stannp-postcards-api-openapi.yml\n      - openapi/stannp-recipients-api-openapi.yml\n  - name: apiKeyQuery\n    type: apiKey\n    in: query\n    parameter_name: api_key\n    description: >-\n\
  \      Append `?api_key={API_KEY}` to the request URL. Documented by Stannp but\n      NOT declared in any OpenAPI in this repo.\n    documented: true\n    in_spec: false\n    source: https://www.stannp.com/us/direct-mail-api/guide\n    risk_note: >-\n      A key in the query string is logged by proxies, CDNs, browser history and\n      server access logs. HTTP Basic is the safer of the two published options.\n  - name: publicKey\n    type: apiKey\n    in: query\n    parameter_name: api_key\n    scope: /v1/qrcode/create only\n    description: >-\n      QR-code generation takes a PUBLIC key rather than the private API key,\n      because the resulting image URL is embedded in mail artwork and rendered by\n      third parties.\n    documented: true\n    in_spec: false\n    source: https://www.stannp.com/us/direct-mail-api/tools\ntransport:\n  https_required: true\n  enforcement: >-\n    Stannp documents that requests made over plain HTTP \"will fail and could\n    suspend your API key\"\
  \ — a stated consequence, not just a redirect.\n  observed_tls: TLSv1.3 on api-eu1.stannp.com and api-us1.stannp.com\n  see_also: security/stannp-domain-security.yml\nkey_management:\n  location: https://app-us1.stannp.com/settings/api\n  ui_only: true\n  rotation_api: none\n  revocation_api: none\n  expiry: none documented\n  scopes: none\n  multiple_keys: not documented\nregional_binding:\n  note: >-\n    A key is issued against a regional account and authenticates only on that\n    region's host — an api-eu1 key will not work against api-us1. This is an\n    auth-relevant fact that is easy to misread as a 401 for a bad key.\n  hosts:\n    - https://api-eu1.stannp.com/v1\n    - https://api-us1.stannp.com/v1\naccount_security:\n  mfa: >-\n    Multi-factor authentication on the Stannp account is listed as a compliance\n    feature on every subscription tier\n    (https://www.stannp.com/us/detailed-pricing). It protects the dashboard, not\n    API calls — the API key alone is sufficient\
  \ for full account access.\nfailure_mode:\n  status: 401\n  body: '{\"success\":false,\"error\":\"You need an API key or token to access this service\"}'\n  observed: '2026-08-13'\n  observed_url: https://api-eu1.stannp.com/v1/openapi.json\n  see_also: errors/stannp-problem-types.yml\noauth:\n  supported: false\n  note: >-\n    No OAuth 2.0, no OpenID Connect, no /.well-known/oauth-authorization-server\n    and no /.well-known/openid-configuration on any host. No scopes artifact is\n    written for this provider because there is no scope surface to record.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stannp/refs/heads/main/authentication/stannp-authentication.yml
summary_line: http/apiKey · 3 schemes
tags:
- Direct Mail
- Postcards
- Letters
- Print
- Physical Mail
- Marketing Automation
- Campaigns
- Address Verification
- SMS
- Webhooks
- Mailing Lists
- Fulfillment
---
