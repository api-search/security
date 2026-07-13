---
api_key_in: []
api_specs:
- filename: tradify-openapi.yml
  format: yaml
  label: Tradify Jobs API (Modeled)
  slug: tradify-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradify/refs/heads/main/openapi/tradify-openapi.yml
- filename: tradify-openapi.yml
  format: yaml
  label: Tradify Customers API (Modeled)
  slug: tradify-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradify/refs/heads/main/openapi/tradify-openapi.yml
- filename: tradify-openapi.yml
  format: yaml
  label: Tradify Quotes API (Modeled)
  slug: tradify-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradify/refs/heads/main/openapi/tradify-openapi.yml
- filename: tradify-openapi.yml
  format: yaml
  label: Tradify Invoices API (Modeled)
  slug: tradify-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradify/refs/heads/main/openapi/tradify-openapi.yml
- filename: tradify-openapi.yml
  format: yaml
  label: Tradify Timesheets API (Modeled)
  slug: tradify-timesheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradify/refs/heads/main/openapi/tradify-openapi.yml
auth_types:
- session
description: ''
kind: authentication
layout: security
method: modeled
name: Tradify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tradify secures its APIs with session across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tradify
provider_slug: tradify
scheme_count: 2
schemes:
- description: MODELED. Session token issued after username/password + MFA sign-in to the Tradify apps. Undocumented and not offered as a public API credential.
  in: header
  modeled: true
  name: sessionAuth
  scheme: bearer
  sources:
  - https://supergood.ai/docs/tradify-api
  type: session
- description: Authentication for Tradify's supported integrations happens on the partner platform. For example, connecting Xero uses Xero's OAuth 2.0 authorization, not a Tradify-issued API credential.
  modeled: false
  name: partnerOAuth
  sources:
  - https://www.tradifyhq.com/xero-and-tradify-addon
  - https://help.tradifyhq.com/hc/en-us/articles/360019239014-Understanding-Xero-and-Tradify-s-Integration
  type: oauth2
slug: tradify-authentication
source_filename: tradify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: modeled\nsource: >-\n  Product/help-centre review plus unofficial third-party proxy descriptions. No\n  official Tradify public API authentication documentation exists.\nsummary:\n  types:\n  - session\n  publicApiKeys: false\n  developerPortal: false\nnotes: >-\n  Tradify does NOT publish a public developer API, so there is no documented,\n  self-serve API authentication (no API keys, no OAuth client registration, no\n  personal access tokens). End users sign in to the Tradify web and mobile apps\n  with a username/password and MFA; the app backend (api.tradifyhq.com) then\n  uses a session token that is not documented for third-party use. Unofficial\n  proxies (e.g. Supergood) obtain access by automating that username/password +\n  MFA sign-in and replaying the resulting session. Supported third-party data\n  exchange is instead handled by Tradify's pre-built accounting/payment\n  integrations, where authentication happens on the partner side\
  \ - for example,\n  the Xero integration is authorized with Xero's own OAuth 2.0 flow, not a\n  Tradify credential.\nschemes:\n- name: sessionAuth\n  type: session\n  in: header\n  scheme: bearer\n  modeled: true\n  description: >-\n    MODELED. Session token issued after username/password + MFA sign-in to the\n    Tradify apps. Undocumented and not offered as a public API credential.\n  sources:\n  - https://supergood.ai/docs/tradify-api\n- name: partnerOAuth\n  type: oauth2\n  modeled: false\n  description: >-\n    Authentication for Tradify's supported integrations happens on the partner\n    platform. For example, connecting Xero uses Xero's OAuth 2.0 authorization,\n    not a Tradify-issued API credential.\n  sources:\n  - https://www.tradifyhq.com/xero-and-tradify-addon\n  - https://help.tradifyhq.com/hc/en-us/articles/360019239014-Understanding-Xero-and-Tradify-s-Integration\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tradify/refs/heads/main/authentication/tradify-authentication.yml
summary_line: session · 2 schemes
tags:
- Job Management
- Trades
- Field Service
- Scheduling
- Quoting
- Invoicing
- Timesheets
- Contractors
- SaaS
---
